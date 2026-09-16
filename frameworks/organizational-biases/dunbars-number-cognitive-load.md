---
id: pm-dunbars-number-cognitive-load
title: "Dunbar's Number & Team Cognitive Load: Limits of Organization & Architecture"
description: "Số Dunbar và Tải trọng Nhận thức (Team Cognitive Load) giải thích chi tiết: Bản chất 3 loại tải trọng não bộ (Intrinsic, Extraneous, Germane) và cách giải phóng năng lực cho đội ngũ kỹ sư"
tags:
  - project-management
  - organizational-biases
  - dunbars-number
  - cognitive-load
  - team-topologies
  - platform-engineering
  - system-architecture
scopePaths:
  - docs/agent-knowledge/frameworks/organizational-biases/
related:
  - pm-organizational-biases-overview
  - pm-conways-law
  - pm-brooks-law
  - pm-space-framework
---

# 👥 Số Dunbar & Tải Trọng Nhận Thức (Team Cognitive Load)

> *"Não người có giới hạn dung lượng RAM cố định. Khi bạn bắt một lập trình viên vừa phải nhớ nghiệp vụ ngân hàng phức tạp, vừa phải đánh vật với 500 dòng cấu hình Kubernetes và vừa phải nhớ 20 quy trình xin quyền nội bộ, não của họ sẽ bị 'Out of Memory' (OOM), dẫn đến bug hàng loạt và kiệt sức!"*  
> — **Matthew Skelton & Manuel Pais**, *Team Topologies* (2019).

<!-- convention-summary-start -->

### Dunbar & Cognitive Load Summary

- **Giới hạn phần cứng sinh học con người (Số Dunbar)**:
  - `5 - 8 người (Two-Pizza Team)`: Giới hạn tối ưu cho một nhóm phối hợp nhịp nhàng, tin tưởng tuyệt đối, không cần slide báo cáo.
  - `15 người`: Bắt đầu phân hóa nhóm nhỏ, xuất hiện ma sát giao tiếp.
  - `50 người (Bộ tộc / Tribe)`: Mọi người còn nhớ mặt nhau, có thể họp chung trong 1 phòng.
  - `150 người (Số Dunbar)`: Giới hạn tối đa mà tổ chức duy trì được bằng quan hệ xã hội trước khi bắt buộc phải dùng luật lệ, quy trình và hệ thống phân cấp cứng nhắc.
- **3 Loại Tải Trọng Nhận Thức (Team Cognitive Load)**:
  1. `Intrinsic Load (Bản chất)`: Kiến thức nền tảng (cú pháp ngôn ngữ, SQL, Git).
  2. `Extraneous Load (Tạp âm rác)`: Rắc rối môi trường dev, cấu hình hạ tầng phức tạp, quy trình hành chính vô nghĩa $\rightarrow$ **Cần triệt tiêu về mức tối thiểu**.
  3. `Germane Load (Nghiệp vụ cốt lõi)`: Giải quyết bài toán kinh doanh, tính năng người dùng $\rightarrow$ **Nơi tạo ra tiền và giá trị thực**.
- **Giải pháp thực chiến**: Xây dựng **Platform Team** và **Internal Developer Platform (IDP)** để biến hạ tầng phức tạp thành các API "1-click", giải phóng 100% dung lượng não bộ của dev cho giá trị kinh doanh.
<!-- convention-summary-end -->

---

## 🧮 1. Các Tầng Số Dunbar Trong Tổ Chức Công Nghệ

Nhà nhân chủng học **Robin Dunbar** (Đại học Oxford) chứng minh kích thước vỏ não người chỉ cho phép duy trì một số lượng mối quan hệ có ý nghĩa nhất định:

```
                                  [ 150 Người ] ──► Giới hạn Dunbar (Bắt buộc tách công ty/chi nhánh)
                                        │
                                  [ 50 Người ]  ──► Bộ tộc (Tribe / Phòng ban lớn)
                                        │
                                  [ 15 Người ]  ──► Squad lớn (Bắt đầu xuất hiện rạn nứt giao tiếp)
                                        │
                                  [ 5 - 8 Người ] ──► TWO-PIZZA TEAM (Hiệu suất vàng!)
```

| Quy mô | Tên gọi | Bản chất vận hành & Hành vi giao tiếp |
| :---: | :--- | :--- |
| **5 - 8 người** | **Two-Pizza Team** | Hai chiếc bánh pizza đủ cho cả nhóm ăn. Standup 10 phút, không cần quản lý trung gian, release tính bằng ngày. |
| **15 người** | **Cụm mở rộng** | Bắt đầu hình thành các "nhóm nhỏ trong nhóm lớn", nảy sinh hiểu lầm, cần Tech Lead điều phối liên tục. |
| **50 người** | **Tribe (Spotify Model)** | Mọi người vẫn nhớ mặt và tên nhau; vẫn có thể cùng nhau chia sẻ một tầm nhìn chung. |
| **150 người** | **Dunbar's Number** | Quá 150 người, não bộ xem những người còn lại là "người lạ". Bắt buộc phải có HR, thủ tục hành chính, chấm công và kiểm soát quyền lực. |

---

## 🧠 2. Mổ Xẻ Chuyên Sâu: 3 Loại Tải Trọng Nhận Thức (Cognitive Load)

Hãy tưởng tượng não bộ của một lập trình viên giống như một thanh **RAM 16GB**. Tại mỗi thời điểm làm việc, thanh RAM này bị phân bổ cho 3 loại tải trọng:

```
┌────────────────────────────────────────────────────────────────────────┐
│               TỔNG DUNG LƯỢNG RAM NÃO BỘ CỦA DEV (16GB)                │
├────────────────────────────────────────────────────────────────────────┤
│                                                                        │
│  [1. INTRINSIC LOAD]       [2. EXTRANEOUS LOAD]   [3. GERMANE LOAD]    │
│  (Kỹ năng nền tảng)        (Tạp âm lãng phí)      (Nghiệp vụ ra tiền)  │
│  - Cú pháp TypeScript      - Fix lỗi Docker/K8s   - Thuật toán tính giá│
│  - Viết truy vấn SQL       - Xin quyền truy cập   - Logic thanh toán   │
│  - Thao tác Git            - Họp hành vô bổ       - Tính thuế VAT      │
│                                                                        │
└────────────────────────────────────────────────────────────────────────┘
```

---

### 🔹 1. Intrinsic Cognitive Load (Tải Trọng Bản Chất)
- **Bản chất**: Là những kiến thức, kỹ năng nền tảng bắt buộc phải có để thực hiện nghề nghiệp.
- **Ví dụ đời thực**: Giống như việc bạn phải **biết đọc chữ, biết đi xe máy, biết dùng đũa**.
- **Trong lập trình**:
  - Biết cú pháp TypeScript, React hook `useEffect`.
  - Biết viết câu lệnh `JOIN` trong PostgreSQL.
  - Biết cách giải quyết Git conflict cơ bản.
- **Đặc điểm**:
  - Không trực tiếp giải quyết bài toán kinh doanh của khách hàng, nhưng thiếu nó thì không thể làm việc được.
  - Chiếm một lượng RAM cố định trong não.
- **Cách tối ưu**:
  - **Tuyển dụng đúng người**: Tuyển dev đã có sẵn kỹ năng nền tảng thay vì tuyển người vào rồi đào tạo lại từ bảng chữ cái.
  - **Giữ công nghệ ổn định**: Đừng mỗi tháng đổi sang một ngôn ngữ/framework mới, sẽ bắt não dev liên tục phải nạp lại Intrinsic Load.

---

### 🔹 2. Extraneous Cognitive Load (Tải Trọng Ngoại Lai / Tạp Âm Rác)
- **Bản chất**: Là toàn bộ những khó khăn, phiền toái, rườm rà do **môi trường làm việc tồi, công cụ phức tạp, hoặc quy trình quan liêu** tạo ra.
- **Ví dụ đời thực**: Bạn muốn lái xe đến chỗ làm (mục tiêu chính), nhưng xe bị xịt lốp, đường ngập nước, GPS chỉ đường sai, và phải dừng lại 5 lần xuất trình giấy tờ ở các trạm kiểm soát vô lý.
- **Trong lập trình**:
  - Cài đặt môi trường dev local mất 3 ngày vì lỗi phiên bản C++ Compiler / `node-gyp`.
  - Để deploy 1 dòng code sửa lỗi, dev phải tự viết và debug 300 dòng file cấu hình `values.yaml` của Kubernetes.
  - Muốn xem log trên Staging phải tạo ticket Jira xin quyền, chờ 3 sếp duyệt qua 2 ngày.
  - Codebase cũ không có tài liệu, mở file ra thấy 1 class dài 4.000 dòng spaghetti, biến đặt tên kiểu `a1, temp, data2`.
- **Đặc điểm**:
  - 💥 **HOÀN TOÀN VÔ NGHĨA VỚI KHÁCH HÀNG!** Khách hàng không bao giờ trả thêm tiền vì dev của bạn đã mất 5 tiếng vật lộn với lỗi Docker.
  - Đây là "kẻ cắp thời gian" và là nguyên nhân số 1 gây ra kiệt sức (Burnout) và nản lòng ở kỹ sư.
- **Cách tối ưu**: **TRIỆT TIÊU TỐI ĐA!** Biến mọi thứ phức tạp thành tự động hoặc cung cấp sẵn dưới dạng nền tảng "1-click".

---

### 🔹 3. Germane Cognitive Load (Tải Trọng Thụ Đắc / Giá Trị Kinh Doanh Cốt Lõi)
- **Bản chất**: Là phần năng lượng trí tuệ dành riêng cho việc **suy nghĩ, giải quyết bài toán nghiệp vụ kinh doanh của khách hàng**.
- **Ví dụ đời thực**: Bạn lái xe an toàn tới buổi đàm phán và dùng $100\%$ trí tuệ để thương thảo bản hợp đồng triệu USD.
- **Trong lập trình**:
  - Tìm ra thuật toán tối ưu để tài xế Grab nhận cuốc xe gần nhất trong 200ms.
  - Xử lý bài toán giao dịch ngân hàng đảm bảo không bao giờ bị trừ tiền 2 lần khi mạng chập chờn (Idempotency).
  - Cài đặt công thức tính thuế thu nhập cá nhân lũy tiến phức tạp cho ứng dụng kế toán.
- **Đặc điểm**:
  - 🌟 **ĐÂY LÀ NƠI DUY NHẤT TẠO RA TIỀN, TÍNH NĂNG VÀ LỢI THẾ CẠNH TRANH CỦA CÔNG TY!**
  - Càng dành nhiều RAM não cho Germane Load, sản phẩm càng ít lỗi logic, trải nghiệm người dùng càng mượt mà.

---

## 💥 3. So Sánh Hai Đội Ngũ: Bị "OOM Não" vs. Được "Giải Phóng Não"

```
[TEAM A: TỔ CHỨC KÉM - BỊ "OOM NÃO"]
┌──────────────────┬──────────────────────────────────────────┬──────────┐
│ Intrinsic (25%)  │       Extraneous Load (65%)              │ Germane  │
│ (Code React)     │       (Vật lộn với K8s, xin quyền, họp)  │ (10%) ⚠️ │
└──────────────────┴──────────────────────────────────────────┴──────────┘
 💥 Kết quả: Dev mệt mỏi rã rời, chỉ còn 10% não để nghĩ về tính năng.
    ==> Tính sai tiền của khách, sót trường hợp biên, bug ngập tràn!

[TEAM B: ÁP DỤNG TEAM TOPOLOGIES & PLATFORM ENGINEERING]
┌──────────────────┬──────────┬──────────────────────────────────────────┐
│ Intrinsic (20%)  │Extraneous│        Germane Load (75%) 🚀             │
│ (Code chuẩn)     │ (5%) ✅  │        (Dành 75% não giải quyết bài toán)│
└──────────────────┴──────────┴──────────────────────────────────────────┘
 🚀 Kết quả: Hạ tầng đã có Platform lo bằng "1-click". Dev tập trung 100%
    sáng tạo tính năng đỉnh cao, release nhanh gấp 5 lần!
```

---

## 🛡️ 4. Bốn Mô Hình Team Chuẩn Trong "Team Topologies" Để Giảm Tải

Để đưa Extraneous Load về mức tối thiểu, cuốn sách *Team Topologies* đề xuất cơ cấu công ty thành 4 loại team:

```
┌────────────────────────────────────────────────────────────────────────┐
│  1. STREAM-ALIGNED TEAM (Nhóm Chuyển giao Giá trị - 80% kỹ sư)        │
│     Chuyên tâm 100% vào nghiệp vụ kinh doanh (Germane Load).          │
│     Ví dụ: Team Thanh Toán, Team Đặt Hàng, Team Giỏ Hàng.             │
├────────────────────────────────────────────────────────────────────────┤
│  ▲                                  ▲                     ▲            │
│  │ Được phục vụ bởi                 │ Được hỗ trợ bởi     │ Tích hợp   │
│                                                                        │
│  2. PLATFORM TEAM                   3. ENABLING TEAM      4. COMPLICATED│
│  (Nhóm Nền tảng)                    (Nhóm Khai vấn)          SUBSYSTEM  │
│  Đóng gói toàn bộ CI/CD,            Cử chuyên gia vào     (Nhóm Chuyên │
│  Kubernetes, Monitoring thành       hướng dẫn team bắt    sâu Thuật toán│
│  "Cổng Tự Phục Vụ" (Self-Service)   nhịp công nghệ mới    Toán học / AI)│
│  giúp Stream team không phải bận    trong 2 tuần rồi rút.               │
│  tâm cấu hình.                                                         │
└────────────────────────────────────────────────────────────────────────┘
```

---

## 🎯 5. Checklist Đánh Giá Dành Cho Tech Lead & Quản Lý

Hãy tự hỏi team của bạn mỗi tuần:
- [ ] Lập trình viên mới mất bao lâu để chạy được code trên máy local? *(Nếu mất quá 1 buổi sáng $\rightarrow$ Extraneous Load quá cao! Cần Dockerize lại ngay)*.
- [ ] Mỗi lần deploy lên Staging/Production mất bao nhiêu thao tác thủ công? *(Nếu phải gõ quá 1 lệnh $\rightarrow$ Cần làm pipeline CI/CD tự động)*.
- [ ] Dev có phải mở hơn 3 màn hình hoặc nhớ hơn 5 tool khác nhau để tìm log lỗi không? *(Cần làm dashboard tập trung Grafana/Datadog)*.
- [ ] Domain của team có quá rộng không? *(Nếu 1 team vừa làm App Mobile, vừa làm Core Backend, vừa trực Cloud $\rightarrow$ Bắt buộc phải tách team theo Bounded Contexts)*.
