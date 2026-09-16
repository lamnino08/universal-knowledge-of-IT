---
id: pm-lehmans-laws
title: "Lehman's Laws of Software Evolution: The Inevitable Decay & Adaptation of Systems"
description: "8 định luật Lehman về sự tiến hóa phần mềm, quy luật suy thoái chất lượng mã nguồn, entropy kiến trúc và chiến lược tái cấu trúc liên tục"
tags:
  - project-management
  - software-engineering
  - lehmans-laws
  - software-evolution
  - technical-debt
  - refactoring
  - system-entropy
scopePaths:
  - docs/agent-knowledge/frameworks/engineering-laws/
related:
  - pm-engineering-laws-overview
  - pm-broken-windows-theory
  - pm-galls-law
  - pm-sunk-cost-fallacy
---

# 🧬 Các Định Luật Lehman Về Tiến Hóa Phần Mềm (Lehman's Laws)

> *"Một chương trình máy bay hay hệ thống kinh doanh không bao giờ thực sự 'hoàn thành'. Hoặc là nó liên tục thay đổi để thích nghi với môi trường sống, hoặc là nó sẽ chết."* — **Meir Lehman**, Giáo sư Điện toán tại Imperial College London (1974 - 1996).

<!-- convention-summary-start -->

### Lehman's Laws Summary

- **The Fundamental Nature of E-Type Systems**: Hệ thống phần mềm thực tế (Evolutionary Systems) luôn gắn liền với môi trường kinh doanh con người. Khi môi trường thay đổi, phần mềm bắt buộc phải biến đổi theo.
- **The Core 3 Laws of System Decay**:
  1. `Continuing Change (Đổi mới liên tục)`: Hệ thống phải liên tục thích ứng, nếu không sẽ mất dần giá trị và bị đào thải.
  2. `Increasing Complexity (Độ phức tạp gia tăng)`: Khi phần mềm tiến hóa, cấu trúc của nó ngày càng rối rắm và suy thoái, TRỪ KHI có công sức chủ động tái cấu trúc (Refactoring).
  3. `Declining Quality (Chất lượng suy giảm)`: Chất lượng của hệ thống sẽ tự động suy thoái theo thời gian nếu không được bảo trì, do các yêu cầu mới làm phá vỡ các giả định thiết kế ban đầu.
- **The Strategic Imperative**: Phải dành từ **$20\% - 30\%$ năng lực (Capacity Allocation)** của mỗi sprint cho công tác dọn dẹp kỹ thuật và refactor để chống lại Entropy phần mềm.
<!-- convention-summary-end -->

---

## 1. 📜 Bối Cảnh Lịch Sử: Công Trình Nghiên Cứu 30 Năm Của Meir Lehman

Trong suốt 3 thập kỷ nghiên cứu các hệ điều hành lớn tại tập đoàn IBM (như OS/360) và các phần mềm công nghiệp toàn cầu, Giáo sư Meir Lehman cùng các cộng sự đã phát hiện ra rằng sự phát triển phần mềm tuân theo các quy luật động học tương tự như **Định luật Nhiệt động lực học thứ hai (Quy luật Tăng Entropy)**:

> Trong một hệ thống kín, độ hỗn loạn (Entropy) sẽ luôn tự động gia tăng theo thời gian. Trong phần mềm, "độ hỗn loạn" chính là **Nợ Kỹ Thuật (Technical Debt)** và **Sự Thoái Hóa Cấu Trúc Kiến Trúc (Architectural Erosion)**.

Lehman phân loại phần mềm thành 3 nhóm:
- **S-Type (Spec-based)**: Giải các bài toán toán học cố định (ví dụ: tính ma trận). Không cần tiến hóa.
- **P-Type (Problem-based)**: Giải bài toán thế giới thực có thể mô hình hóa (ví dụ: cờ vua). Ít tiến hóa.
- **E-Type (Evolutionary)**: Phần mềm doanh nghiệp, ngân hàng, thương mại điện tử, game gắn liền với hoạt động của con người. **Bắt buộc tuân theo 8 định luật Lehman**.

---

## 2. 🏛️ Chi Tiết 8 Định Luật Tiến Hóa Phần Mềm Của Lehman

```
┌────────────────────────────────────────────────────────────────────────┐
│                  8 ĐỊNH LUẬT TIẾN HÓA PHẦN MỀM LEHMAN                  │
├────────────────────────────────────────────────────────────────────────┤
│                                                                        │
│  [1. Tiếp tục Thay đổi]          ──► Bắt buộc phải thay đổi để sống    │
│  [2. Độ phức tạp Gia tăng]      ──► Code tự động rối rắm theo thời gian│
│  [3. Tự điều chỉnh Phát triển]   ──► Năng suất team có xu hướng ổn định│
│  [4. Bảo toàn Độ quen thuộc]    ──► Thay đổi quá nhanh sẽ gây sốc/bug │
│  [5. Bảo toàn Tính tăng trưởng] ──► Mỗi release chỉ thêm lượng vừa phải│
│  [6. Tiếp tục Tăng trưởng]       ──► Tính năng người dùng ngày càng đòi│
│  [7. Chất lượng Suy thoái]       ──► Code tự thoái hóa nếu không sửa   │
│  [8. Hệ thống Phản hồi]         ──► Quá trình dev là chu trình hồi tiếp│
│                                                                        │
└────────────────────────────────────────────────────────────────────────┘
```

| Định luật | Tên tiếng Anh | Ý nghĩa thực tiễn & Lời khuyên cho Tech Lead |
| :--- | :--- | :--- |
| **I. Tiếp tục Thay đổi** | *Continuing Change* | Đừng bao giờ mong đợi một ngày "code xong xuôi và không cần động vào nữa". Mọi dòng code đều là tạm thời. |
| **II. Độ phức tạp Tăng** | *Increasing Complexity* | Mỗi commit mới đều làm tăng một chút độ phức tạp của codebase. Nếu không refactor định kỳ, chi phí phát triển tính năng mới sẽ tăng theo hàm số mũ. |
| **III. Tự điều chỉnh** | *Self Regulation* | Tốc độ release của dự án phản ánh cấu trúc tổ chức và văn hóa công ty, rất khó để ép tăng tốc đột biến chỉ bằng khẩu hiệu. |
| **IV. Bảo toàn Quen thuộc** | *Conservation of Familiarity* | Nếu release quá nhiều tính năng lớn cùng lúc trong 1 version, cả người dùng lẫn đội ngũ vận hành sẽ bị quá tải nhận thức, dẫn đến khủng hoảng hỗ trợ. |
| **V. Bảo toàn Tăng trưởng** | *Conservation of Growth* | Khối lượng thay đổi trung bình trong mỗi phiên bản thường có giới hạn tự nhiên, vượt quá ngưỡng này sẽ sinh ra hàng loạt lỗi hồi quy (Regression Bugs). |
| **VI. Tiếp tục Tăng trưởng** | *Continuing Growth* | Người dùng không bao giờ hài lòng lâu dài. Nhu cầu chức năng của hệ sinh thái sẽ liên tục phình to. |
| **VII. Suy giảm Chất lượng** | *Declining Quality* | Một hệ thống không có bug hôm nay sẽ trở thành hệ sinh thái đầy lỗi sau 2 năm vì các thư viện phụ thuộc, hệ điều hành và kỳ vọng người dùng đều đã đổi khác. |
| **VIII. Hệ thống Phản hồi** | *Feedback System* | Việc phát triển phần mềm là một chu trình phản hồi nhiều tầng. Bạn phải đo lường telemetry và quan sát hành vi người dùng liên tục. |

---

## 3. 📉 Động Lực Học Suy Thoái Kiến Trúc (Architectural Erosion)

Khi một dự án mới bắt đầu (Day 1), kiến trúc rất thanh lịch và rõ ràng. Nhưng theo thời gian và áp lực deadline:

```
[Day 1: Clean Architecture]        [Year 3: Spaghetti Architecture]
     Layer UI                            Layer UI ─────────┐ (Shortcut)
        │                                   │              ▼
     Layer Service                       Layer Service ──► Direct DB Query
        │                                   │              ▲
     Layer Repository                    Layer Repository ─┘
        │                                   │
     Database                            Database
  (Phân lớp nghiêm ngặt)           (Vá víu, phá vỡ trừu tượng)
```

1. **Hotfix khẩn cấp lúc nửa đêm**: Viết câu lệnh truy vấn trực tiếp vào DB ngay tại tầng giao diện (UI) để cứu hỏa.
2. **Quy tắc ngoại lệ (Exceptions)**: "Chỉ làm tạm thế này cho khách hàng VIP X, sau này sẽ sửa lại sau" (nhưng không bao giờ sửa).
3. **Phá vỡ Domain Boundary**: Service A đọc trộm bảng dữ liệu của Service B mà không qua API.

---

## 4. 🛡️ Chiến Lược Ứng Phó: Vận Hành Ngăn Ngừa Suy Thoái

### 1. Phân Bổ Năng Lực Cố Định (Capacity Allocation 70-20-10)
Không để Technical Debt cạnh tranh trực tiếp với Product Features trong Sprint Planning:
- **70%**: Tính năng kinh doanh mới (Product Roadmap).
- **20%**: Nâng cấp kiến trúc, Refactoring, trả nợ kỹ thuật (Architectural Health).
- **10%**: Nghiên cứu, tối ưu hạ tầng CI/CD, thử nghiệm công nghệ mới (Innovation).

### 2. Quy Tắc Hướng Đạo Sinh (The Boy Scout Rule)
> *"Luôn để lại khu cắm trại sạch sẽ hơn lúc bạn tìm thấy nó."*  
Khi mở một file code ra để sửa bug, hãy tranh thủ dọn dẹp biến thừa, tách hàm quá dài hoặc viết thêm 1 bài Unit Test trước khi commit.

### 3. Fitness Functions (Kiểm Tra Tính Toàn Vẹn Kiến Trúc Tự Động)
Sử dụng các công cụ như `ArchUnit` (Java), `Dependency-cruiser` (NodeJS) trong pipeline CI để tự động chặn các commit vi phạm kiến trúc:
```typescript
// Chặn UI gọi trực tiếp vào DB
forbidden: [
  {
    from: { path: "^src/ui" },
    to: { path: "^src/database" }
  }
]
```
