---
id: ak-ui-ux-public-profile-persona-vs-private-workspace-separation-pattern
title: 'Public Profile Persona vs Private Workspace Separation Pattern'
description: 'Phân tách rạch ròi giữa Public Persona (Hồ sơ thị hiếu công khai như Tủ game, Phim yêu thích) và Private Workspace (Tiện ích cá nhân như Đã lưu, Lịch sử) khi xem trang thành viên trên toàn bộ các Spoke (Boardgame, Cinema/Movie).'
tags:
  - ui-ux
  - public-profile
  - persona
  - private-workspace
  - boardgame
  - movie
  - cinema
scopePaths:
  - workspace/web/app/(main)/social/members/[user_slug]/
  - workspace/web/app/(main)/social/members/[user_slug]/_components/tabs/CinemaProfileTab.tsx
  - workspace/web/app/(main)/social/members/[user_slug]/liked/_components/MovieLikedList.tsx
  - workspace/back-end/src/controllers/LikeController.ts
  - workspace/back-end/src/routes/v1/common/like/getLikedItemsRoute.ts
---

# Public Profile Persona vs Private Workspace Separation Pattern

**Category:** ui-ux  
**Type:** Continuous Self-Learning Pattern & Architecture Standard  
**Recorded At:** 2026-10-13  
**Scope:** Ecosystem-wide (`@spoke/boardgame`, `@spoke/movie`, Social Profile `/social/members/[user_slug]`)  

---

## 🔍 1. Problem & Context (The "Private Workspace Leak" Anti-Pattern)

Khi người dùng A truy cập trang hồ sơ cá nhân của người dùng B (`/social/members/[user_slug]`):
1. **Rò rỉ ngữ cảnh cá nhân (Context Leak)**: Các tab như *Đã lưu (Saved / Bookmarks)* và *Lịch sử xem (History)* vốn là **tiện ích cá nhân (Private Workspace)** của người đang đăng nhập. Nếu để lộ ra khi xem trang người khác, hệ thống hoặc truy vấn dữ liệu của chính người xem (gây nhầm lẫn trầm trọng: "Ủa sao trang bạn này lại hiện phim/game mình vừa lưu?"), hoặc bị rỗng vô nghĩa.
2. **Ẩn giấu tài sản xã hội (Social Persona Hidden)**: Thay vì làm nổi bật thị hiếu, phong cách và đóng góp của chủ hồ sơ (như Tủ Boardgame cá nhân, hay Gu xem phim qua các phim họ đã yêu thích), giao diện trước đây lại giấu các tài sản này đi đối với người ngoài.
3. **Lệch pha nhận thức (Empty State Mismatch)**: Các câu thông báo rỗng (Empty state) mang văn phong thúc giục chính chủ thao tác (VD: *"Bạn chưa lưu phim nào, hãy khám phá ngay"*), gây cảm giác kỳ quặc khi người ngoài đang ghé thăm một profile trống.

---

## 🏛️ 2. Core Design Principles

### Principle 1: Public Persona vs Private Workspace
| Khái niệm | Định nghĩa | Ai thấy? | Ví dụ trong Ineffable |
| :--- | :--- | :--- | :--- |
| **Public Persona** | *Bộ mặt & thị hiếu xã hội*: Thể hiện gu giải trí, danh mục sở hữu, thành tựu và hoạt động cộng đồng của thành viên. | Mọi người (`isOwner = true/false`) | Tủ game cá nhân (Boardgame Collection), Phim yêu thích (Liked Movies), Buổi chơi đã tham gia / host. |
| **Private Workspace** | *Không gian tiện ích cá nhân*: Công cụ lưu trữ tạm thời, đánh dấu theo dõi riêng tư và nhật ký hoạt động. | Chỉ chính chủ (`isOwner = true`) | Phim đã lưu (`saved`), Game đã đánh dấu (`bookmarks`), Lịch sử duyệt (`history`). |

### Principle 2: Asymmetric Privacy & View-Only Safeguards
- Khi `!isOwner`:
  - Ẩn triệt để tất cả các tab và luồng tương tác thuộc nhóm Private Workspace.
  - Các danh mục thuộc Public Persona phải được chuyển sang chế độ **View-Only**: ẩn các nút hành động chỉnh sửa, xóa, đồng bộ hóa (Sync BGG), hoặc quản lý vị trí tủ.
  - Empty state phải chuyển sang góc nhìn người thứ ba (Third-person perspective).

---

## 🛠️ 3. Implementation Matrix Across Spokes

### 3.1 Spoke Boardgame (`boardgame.ineffable.test`)
- **Khi là chính chủ (`isOwner = true`)**:
  - Tab *Tủ game cá nhân*: Cho phép CRUD, chỉnh sửa trạng thái chơi, thêm ghi chú riêng tư, đồng bộ BoardGameGeek (BGG).
  - Tab *Đã lưu* & *Lịch sử*: Hiển thị danh sách bookmark và game đã xem gần đây.
- **Khi là người ngoài xem (`isOwner = false`)**:
  - **Ẩn hoàn toàn**: Tab *Đã lưu* & *Lịch sử*.
  - **Hiển thị**: Tab *Tủ game của [Tên]* (`boardgame_other_collection`): Chế độ View-Only, chỉ hiển thị danh mục game và thông tin cơ bản.
  - **Sessions**: Hiển thị danh sách các buổi Host / Session mà thành viên này từng đứng ra tổ chức hoặc tham gia.
  - **Backend Support**: `GET /boardgame/collection` sử dụng `optionalAuth`, chấp nhận query param `user_id` / `user_slug` để trả về tủ game của chủ tài khoản thay vì mặc định lấy `c.req.user.id`.

### 3.2 Spoke Movie / Cinema (`movie.ineffable.test`)
- **Khi là chính chủ (`isOwner = true`)**:
  - Tab *Phim yêu thích* (`liked`): Xem danh sách phim đã bấm Like.
  - Tab *Phim đã lưu* (`saved`): Danh sách phim lưu xem sau.
  - Tab *Lịch sử xem* (`history`): Nhật ký xem phim cá nhân.
- **Khi là người ngoài xem (`isOwner = false`)**:
  - **Ẩn hoàn toàn**: Tab `saved` và `history` (bảo vệ quyền riêng tư trải nghiệm xem).
  - **Hiển thị duy nhất**: Tab **Phim yêu thích của [Tên]** (`cinema_other_liked`) - Hoạt động như một **Taste Showcase (Bộ sưu tập gu điện ảnh)** của người đó.
  - **Backend Support**:
    - Route `GET /like` ([getLikedItemsRoute.ts](file:///d:/lamnino/personal/ineffable/workspace/back-end/src/routes/v1/common/like/getLikedItemsRoute.ts)) chuyển sang `optionalAuth`.
    - Controller [LikeController.ts](file:///d:/lamnino/personal/ineffable/workspace/back-end/src/controllers/LikeController.ts) phân giải:
      ```typescript
      let targetUserId = c.req.user?.id;
      if (params.user_id) targetUserId = params.user_id;
      else if (params.user_slug) {
        const u = await userService.getProfileBySlug(params.user_slug);
        targetUserId = u?.id;
      }
      ```
    - Validation schema [LikeFilterConfig.ts](file:///d:/lamnino/personal/ineffable/workspace/packages/shared/validation/common/LikeFilterConfig.ts) mở rộng thêm `.extend({ user_id: z.string().optional(), user_slug: z.string().optional() })`.
  - **Frontend Support**:
    - [CinemaProfileTab.tsx](file:///d:/lamnino/personal/ineffable/workspace/web/app/(main)/social/members/[user_slug]/_components/tabs/CinemaProfileTab.tsx): Nhận `isOwner` và `user`. Khi `!isOwner`, chỉ render tab `liked` với nhãn `Phim yêu thích của ${user.name}`.
    - [MovieLikedList.tsx](file:///d:/lamnino/personal/ineffable/workspace/web/app/(main)/social/members/[user_slug]/liked/_components/MovieLikedList.tsx): Truyền `targetUserId`, `targetUserSlug` xuống `LikedItemsDataListView` và render `otherEmptyState` khi danh sách trống.

---

## 💬 4. UX Writing & i18n Standards (Duolingo Style)

Tuân thủ nghiêm ngặt quy định dự án tại `AGENTS.md`:
1. **Tuyệt đối KHÔNG inline ternary locale** (`locale === 'vi' ? ... : ...`). Toàn bộ string phải nằm trong từ điển `@shared/lib/i18n`.
2. **Tuyệt đối KHÔNG emoji/icon trong string i18n**: Emoji và biểu tượng thuộc về UI Layer qua component (Lucide/SVG). Chuỗi i18n phải là **Pure Text**.
3. **Văn phong Duolingo**: Tươi vui, hờn dỗi nhẹ nhàng, cà khịa thân mật, góc nhìn người thứ ba (Third-person):

| Ngữ cảnh | Key i18n | Tiếng Việt (`vi.ts`) | English (`en.ts`) |
| :--- | :--- | :--- | :--- |
| **Boardgame Empty** | `boardgame_other_empty_title` | `{name} chưa thêm tựa game nào vào tủ nè!` | `{name} hasn't added any games to their shelf yet!` |
| | `boardgame_other_empty_desc` | `Chờ {name} sắm game mới rồi quay lại mượn chơi ké nha!` | `Wait for {name} to bring some new games, then drop by to borrow and play!` |
| **Cinema Liked Tab** | `cinema_other_liked` | `Phim yêu thích của {name}` | `{name}'s Favorite Movies` |
| **Cinema Liked Empty** | `cinema_other_liked_empty_title` | `Chưa có phim nào lọt vào mắt xanh của {name} hết trơn!` | `No movies have caught {name}'s eye yet!` |
| | `cinema_other_liked_empty_desc` | `Gu chọn phim hơi khó tính hoặc {name} đang bận cày phim mà quên thả tim đó mà.` | `Either high standards, or {name} is just binge-watching and forgot to drop a heart.` |

---

## 🚫 5. Anti-Patterns & Regressions to Avoid

1. **Anti-pattern 1: Blind Context Assumption in API**:
   - *Sai*: Chỉ lấy `c.req.user.id` trong route được chia sẻ công khai.
   - *Đúng*: Kiểm tra `params.user_id` / `params.user_slug` trước; nếu có, tra cứu public profile của người đó; chỉ fallback về `c.req.user.id` khi không truyền param và có authentication.
2. **Anti-pattern 2: Client-side `isOwner` Hydration Flashing**:
   - *Sai*: Dùng hook `useCurrentUser()` trong Client Component để render có điều kiện các Tab. Khi SSR, client chưa có user -> Server render khác Client -> Hydration Mismatch.
   - *Đúng*: Tính toán `isOwner = currentUser?.id === targetUser.id` từ Server Component (`layout.tsx` / `page.tsx`) và truyền xuống dưới dạng prop đã kiểm chứng.
3. **Anti-pattern 3: Hiển thị Private Buttons ở chế độ View-Only**:
   - *Sai*: Người lạ thấy nút "Thêm vào tủ", "Xóa khỏi danh sách", "Đồng bộ BGG".
   - *Đúng*: Ẩn triệt để toàn bộ action buttons hoặc chuyển sang chế độ Bookmarking/Lưu về tủ của chính người xem.
4. **Anti-pattern 4: Fallback to Authenticated User on Invalid/Non-existent Slug (Context Leakage)**:
   - *Sai*: Khi client truyền `user_slug` nhưng không tìm thấy user (`targetUser = undefined`), controller lại fallback `targetUserId = c.req.user?.id`. Hậu quả: Người đang đăng nhập xem hồ sơ một slug sai/đã xóa sẽ nhìn thấy dữ liệu cá nhân của chính mình trên trang đó!
   - *Đúng*: Nếu `user_slug` được truyền mà không tìm thấy user, trả về mảng rỗng `[]` ngay lập tức để UI render Empty State, tuyệt đối không fallback về `c.req.user?.id`. Chỉ fallback khi client hoàn toàn không truyền target identifier nào (tự truy vấn cho chính mình).
5. **Anti-pattern 5: Trả về trường nhạy cảm trong User Profile**:
   - *Sai*: Trả về raw object từ database chứa `password_hash`, `provider_user_id` hay token.
   - *Đúng*: Luôn sanitize xóa `password_hash`, `provider_user_id` trong mọi profile controller (`getProfile`, `getProfileBySlug`, `getProfileByCode`). Các route polymorphic (`GET /like`) chỉ làm giàu metadata công khai của entity (`Movie`, `Boardgame`) qua `enrichLikedItem`, không gắn kèm dữ liệu tài khoản cá nhân.

