---
id: pm-broken-windows-theory
title: "Broken Windows Theory: Preventing Codebase Entropy & Cultural Degradation"
description: "Thuyết Cửa Sổ Vỡ trong phát triển phần mềm, cơ chế tâm lý hoại tử mã nguồn, lây lan nợ kỹ thuật và văn hóa Zero-Tolerance đối với code bẩn"
tags:
  - project-management
  - software-engineering
  - broken-windows-theory
  - clean-code
  - code-quality
  - technical-debt
  - team-culture
scopePaths:
  - docs/agent-knowledge/frameworks/engineering-laws/
related:
  - pm-engineering-laws-overview
  - pm-lehmans-laws
  - pm-kernighans-law
  - pm-goodharts-law
---

# 🪟 Thuyết Cửa Sổ Vỡ Trong Kỹ Nghệ Phần Mềm (Broken Windows Theory)

> *"Đừng để lại bất kỳ 'cửa sổ vỡ' nào (những đoạn code bẩn, thiết kế tồi, test bị skip, hay warning bị làm lơ). Hãy sửa chữa chúng ngay khi phát hiện. Nếu không kịp sửa triệt để, hãy phong tỏa hoặc đánh dấu rõ ràng. Đừng để sự bỏ bê trở thành thói quen!"*  
> — **Andrew Hunt & David Thomas**, *The Pragmatic Programmer* (1999).

<!-- convention-summary-start -->

### Broken Windows Theory Summary

- **The Psychological Mechanism of Code Rot**: Khi một lập trình viên bước vào một file code đã có sẵn 5 đoạn copy-paste bẩn và biến đặt tên vô nghĩa, não bộ tự động cấp quyền: *"File này vốn đã rác rưởi rồi, mình thêm một đoạn bẩn nữa cũng chẳng sao!"*. Ngược lại, trong một codebase sạch không tì vết, ai cũng sẽ rất cẩn trọng.
- **The Domino Effect of Neglect**: Một cửa sổ vỡ không được sửa chữa sẽ dẫn đến cửa sổ thứ hai bị đập vỡ, rồi cả tòa nhà bị vẽ bậy, và cuối cùng trở thành khu ổ chuột hoang phế (Codebase Abandonment).
- **The Cultural Fixes**:
  1. `Zero Tolerance for Broken Builds & Skipped Tests`: Pipeline CI đỏ là tình huống khẩn cấp P0 của cả team.
  2. `The Boy Scout Rule`: Luôn dọn sạch hơn lúc mới vào.
  3. `Lint & Strict Format as Code Guards`: Tự động hóa việc giữ gìn trật tự bằng máy móc, loại bỏ tranh cãi chủ quan của con người.
<!-- convention-summary-end -->

---

## 1. 📜 Nguồn Gốc Xã Hội Học Đến Kỹ Thuật Phần Mềm

Năm 1982, hai nhà xã hội học **James Q. Wilson** và **George L. Kelling** công bố nghiên cứu về tội phạm học tại New York:
- Nếu một tòa nhà có một ô cửa sổ bị nứt vỡ mà không ai thay thế, người đi đường sẽ kết luận rằng **"ở đây không có ai chịu trách nhiệm, không ai quan tâm cả"**.
- Chẳng mấy chốc, những ô cửa sổ khác sẽ bị ném đá vỡ tiếp. Kẻ xấu bắt đầu tụ tập, rác rưởi bị vứt bừa bãi và cả khu phố nhanh chóng rơi vào cảnh vô pháp luật.

Năm 1999, hai tác giả cuốn sách kinh điển *The Pragmatic Programmer* đã áp dụng trực tiếp mô hình này vào mã nguồn phần mềm:
> Mã nguồn không tự nhiên xấu đi vì máy tính, nó bị thoái hóa bởi **sự xói mòn tâm lý trách nhiệm của chính những người kỹ sư**.

---

## 2. 🔍 Vòng Xoáy Hoại Tử Codebase (The Codebase Rot Cycle)

```
        ┌────────────────────────────────────────────────────────┐
        │ 1. Một "Cửa Sổ Vỡ" Xuất Hiện                           │
        │    - 1 file thiếu unit test                           │
        │    - 1 biến `any` trong TypeScript                    │
        │    - 1 đoạn hard-code credential để test nhanh        │
        └──────────────────────────┬─────────────────────────────┘
                                   │
                                   ▼
        ┌────────────────────────────────────────────────────────┐
        │ 2. Lây Lan Tâm Lý Buông Xuôi (Moral Hazard)           │
        │    - Kỹ sư khác: "Thằng trước làm ẩu được thì sao      │
        │      mình phải tốn công viết test chỉn chu?"          │
        └──────────────────────────┬─────────────────────────────┘
                                   │
                                   ▼
        ┌────────────────────────────────────────────────────────┐
        │ 3. Codebase Rơi Vào Vùng Ổ Chuột (Slum Area)           │
        │    - Không ai dám nhận trách nhiệm refactor            │
        │    - Thời gian sửa bug tăng từ 1 giờ lên 3 ngày        │
        │    - Kỹ sư giỏi chán nản nghỉ việc (Brain Drain)       │
        └────────────────────────────────────────────────────────┘
```

---

## 3. 🚨 Những "Cửa Sổ Vỡ" Phổ Biến Nhất Cần Quét Sạch Ngay

| Loại Cửa Sổ Vỡ | Biểu hiện thường gặp | Hậu quả sau 6 tháng | Giải pháp triệt để |
| :--- | :--- | :--- | :--- |
| **Flaky Tests** | Test thỉnh thoảng fail ngẫu nhiên, dev chỉ việc bấm `Re-run CI` cho qua. | Cả team bỏ qua kết quả CI, bug thật lọt thẳng lên Production. | Cách ly (Quarantine) test flaky ngay lập tức, sửa trong 24h hoặc xóa bỏ. |
| **Compiler Warnings** | Build hiện ra hàng trăm dòng `Warning: unused variable / deprecated`. | Warning che lấp các cảnh báo nguy hiểm thực sự. | Bật cờ `warnings-as-errors` trong compiler / linter. |
| **TODO / FIXME Mồ côi** | `// TODO: Sửa đoạn này sau khi release` (từ 3 năm trước). | Mã nguồn ngập tràn lời hứa suông, giảm tính minh bạch. | Gắn Issue ID cụ thể `// TODO(PROJ-123): ...` hoặc xóa comment nếu không làm. |
| **TypeScript `any`** | Dùng `any` hoặc `@ts-ignore` để tắt kiểm tra kiểu dữ liệu cho nhanh. | Mất toàn bộ lợi thế Type-safety, runtime crash bất ngờ. | Bật `noImplicitAny` và cấm merge PR có `@ts-ignore` không có giải trình. |

---

## 4. 🛡️ Chiến Lược Giữ Gìn Khu Phố Code Sạch Sẽ

```typescript
// Ví dụ: Thiết lập cổng bảo vệ CI tự động ngăn chặn "Cửa Sổ Vỡ"
// package.json script
{
  "scripts": {
    "typecheck": "tsc --noEmit",
    "lint": "eslint . --max-warnings 0", // Không chấp nhận dù chỉ 1 warning!
    "test:coverage": "jest --coverage --coverageThreshold='{\"global\":{\"lines\":80}}'"
  }
}
```

### 1. Phục Hồi Cửa Sổ Tức Thì (Immediate Remediation)
Khi bạn phát hiện một bug hay một đoạn code thối:
- Nếu sửa mất dưới **15 phút**: Hãy sửa ngay trong commit hiện tại.
- Nếu việc sửa chữa đòi hỏi tái cấu trúc lớn: Hãy tạo ngay một Ticket trên Jira/Linear, mô tả rõ rủi ro và đưa vào Sprint Backlog kế tiếp. Tuyệt đối không âm thầm bỏ qua.

### 2. Tôn Vinh Văn Hóa Dọn Dẹp (Celebrate Janitorial Work)
Đừng chỉ khen ngợi những kỹ sư "làm ra tính năng mới hào nhoáng". Hãy khen ngợi và ghi nhận công khai những kỹ sư:
- Giảm thời gian chạy CI từ 15 phút xuống 3 phút.
- Xóa được 5000 dòng code thừa (Dead Code).
- Nâng cấp phiên bản thư viện lỗi thời.
