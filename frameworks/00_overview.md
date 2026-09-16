---
id: pm-frameworks-overview
title: 'Software Project Management & Engineering Mental Models Overview'
description: 'Toàn cảnh các định luật, mô hình tư duy và phương pháp luận quản lý dự án phần mềm hiện đại'
tags:
  - project-management
  - engineering-management
  - mental-models
  - frameworks
  - estimation
  - prioritization
  - flow-efficiency
  - dora
scopePaths:
  - docs/agent-knowledge/frameworks/
related:
  - capacity-allocation-overview
  - pm-time-estimation-overview
  - pm-prioritization-overview
  - pm-flow-efficiency-overview
  - pm-organizational-biases-overview
  - pm-engineering-metrics-overview
  - pm-engineering-laws-overview
---

# 🌐 Software Project Management & Engineering Mental Models

<!-- convention-summary-start -->

### PM Frameworks & Mental Models Summary

- **Core Architecture / Purpose**: Master systemic index and directory of modern software project management principles, engineering laws, prioritization frameworks, system evolution dynamics, and delivery telemetry.
- **The 6 Dedicated Category Sub-domains**:
  1. `Time & Estimation` (`time-estimation/`): [Brooks' Law](./time-estimation/brooks-law.md), [Hofstadter's Law](./time-estimation/hofstadter-law.md), [Parkinson's Law](./time-estimation/parkinsons-law.md), [Cone of Uncertainty](./time-estimation/cone-of-uncertainty.md), [Ninety-Ninety Rule](./time-estimation/ninety-ninety-rule.md), [Student Syndrome](./time-estimation/student-syndrome.md).
  2. `Scope & Prioritization` (`prioritization/`): [Iron Triangle](./prioritization/iron-triangle.md), [RICE Scoring](./prioritization/rice-scoring.md), [WSJF & Cost of Delay](./prioritization/wsjf-cost-of-delay.md), [Kano Model](./prioritization/kano-model.md), [Pareto 80/20 Principle](./prioritization/pareto-principle.md).
  3. `Flow Efficiency & Systems` (`flow-efficiency/`): [Theory of Constraints](./flow-efficiency/theory-of-constraints.md), [Little's Law & WIP](./flow-efficiency/littles-law-and-wip.md), [Lead Time vs. Cycle Time](./flow-efficiency/lead-time-vs-cycle-time.md), [Kingman's Formula & Slack Time](./flow-efficiency/kingmans-formula.md), [Amdahl's Law](./flow-efficiency/amdahls-law.md).
  4. `Organizational Biases` (`organizational-biases/`): [Conway's Law](./organizational-biases/conways-law.md), [Goodhart's Law](./organizational-biases/goodharts-law.md), [Sunk Cost Fallacy](./organizational-biases/sunk-cost-fallacy.md), [Law of Triviality / Bike-shedding](./organizational-biases/law-of-triviality.md), [Chesterton's Fence](./organizational-biases/chestertons-fence.md), [Dunbar's Number & Cognitive Load](./organizational-biases/dunbars-number-cognitive-load.md), [The Peter Principle](./organizational-biases/peter-principle.md).
  5. `Engineering & Architecture Laws` (`engineering-laws/`): [Hyrum's Law](./engineering-laws/hyrums-law.md), [Postel's Law](./engineering-laws/postels-law.md), [Lehman's Laws](./engineering-laws/lehmans-laws.md), [Kernighan's Law](./engineering-laws/kernighans-law.md), [Gall's Law](./engineering-laws/galls-law.md), [Broken Windows Theory](./engineering-laws/broken-windows-theory.md).
  6. `Value Delivery Telemetry` (`engineering-metrics/`): [DORA Metrics](./engineering-metrics/dora-metrics.md), [SPACE Framework](./engineering-metrics/space-framework.md).
- **Scope & Code Paths**: Applied across cross-functional delivery, sprint governance, architecture design, and operational excellence in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Tại sao Kỹ sư Phần mềm cần Nắm vững Mô hình Quản lý & Định luật Kỹ nghệ?

Lập trình giỏi (Software Craftsmanship) chỉ giải quyết bài toán: **"Làm sao để hệ thống chạy đúng và sạch?"**. Tuy nhiên, một dự án phần mềm thành công đòi hỏi trả lời những câu hỏi lớn hơn ở tầng hệ thống:
- *Tại sao thêm người vào dự án đang trễ hạn lại khiến nó trễ hơn nữa? (Brooks' Law)*
- *Làm sao để biết tính năng nào nên làm trước giữa hàng chục yêu cầu từ Product? (RICE, WSJF, Pareto)*
- *Vì sao lập trình viên code rất nhanh nhưng sản phẩm vẫn mất hàng tháng mới đến tay người dùng? (Little's Law, Kingman)*
- *Tại sao kiến trúc hệ thống lại vô tình biến thành bản sao cấu trúc phòng ban công ty? (Conway's Law)*
- *Tại sao một API không đổi tài liệu nhưng vẫn làm sập client khi nâng cấp? (Hyrum's Law)*
- *Tại sao những đoạn code quá "thông minh" lại trở thành tử địa khi gỡ lỗi lúc nửa đêm? (Kernighan's Law)*

> **Mô hình Tư duy (Mental Models)** và **Các Định luật Kỹ nghệ (Engineering Laws)** là các lăng kính trừu tượng giúp Tech Lead, Engineering Manager và Kỹ sư nhìn thấu bản chất của sự phức tạp, đưa ra quyết định có căn cứ và tránh lặp lại những thất bại kinh điển của ngành công nghệ trong 50 năm qua.

---

## 2. 🏛️ 6 Trụ Cột Quản Lý Dự Án & Kỹ Nghệ Phần Mềm Hiện Đại

```
┌───────────────────────────────────────────────────────────────────────────────────┐
│              6 TRỤ CỘT QUẢN TRỊ DỰ ÁN & KỸ NGHỆ PHẦN MỀM HIỆN ĐẠI                 │
├───────────────────────────────────────────────────────────────────────────────────┤
│                                                                                   │
│  [1. Ước lượng & Thời gian]              [2. Cân đối & Ưu tiên]                   │
│  - Brooks' Law (Bùng nổ giao tiếp)       - Iron Triangle (Tam giác sắt Agile)     │
│  - Hofstadter's Law (Unknowns)           - RICE Scoring (Định lượng giá trị)      │
│  - Parkinson's Law (Timeboxing)          - WSJF / Cost of Delay (Kinh tế SAFe)    │
│  - Cone of Uncertainty (Dung sai)        - Kano Model (Kỳ vọng khách hàng)        │
│  - Ninety-Ninety Rule (Bẫy 10% cuối)     - Pareto 80/20 (The Vital Few)           │
│  - Student Syndrome (Hội chứng học sinh)                                          │
│                                                                                   │
│               ─────────────────────────────────────────────                       │
│                                                                                   │
│  [3. Dòng chảy & Điểm nghẽn]             [4. Tổ chức & Bẫy Tâm lý]                │
│  - Theory of Constraints (TOC)           - Conway's Law (Kiến trúc & Team)        │
│  - Little's Law & WIP Limits             - Goodhart's Law (Bẫy lách KPI)          │
│  - Lead Time vs. Cycle Time              - Sunk Cost Fallacy (Cắt lỗ dự án)       │
│  - Kingman's Formula (The 100% Trap)     - Law of Triviality (Bike-shedding)      │
│  - Amdahl's Law (Trần tăng tốc)          - Chesterton's Fence (Legacy Code)       │
│                                          - Dunbar's Number (Cognitive Load)       │
│                                          - The Peter Principle (Thang IC vs EM)   │
│                                                                                   │
│               ─────────────────────────────────────────────                       │
│                                                                                   │
│  [5. Kỹ nghệ & Kiến trúc Mã nguồn]       [6. Đo lường Hiệu suất Chuyển giao]      │
│  - Hyrum's Law (Giao tiếp ngầm API)      - 4 DORA Metrics (Tốc độ & Ổn định)      │
│  - Postel's Law (Robustness Principle)   - SPACE Framework (Năng suất toàn diện)  │
│  - Lehman's Laws (Tiến hóa phần mềm)                                              │
│  - Kernighan's Law (Nghịch lý Debug)                                              │
│  - Gall's Law (Tiến hóa từ đơn giản)                                              │
│  - Broken Windows Theory (Code bẩn)                                               │
│                                                                                   │
└───────────────────────────────────────────────────────────────────────────────────┘
```

---

## 3. 🔄 Bản đồ Dòng chảy Giá trị (From Idea to Production)

Cách 6 trụ cột phối hợp nhịp nhàng trong suốt vòng đời của một hệ thống:

```
[Khởi tạo Ý tưởng & Backlog]
       │
       ▼
[Đánh giá Ưu tiên (Trụ cột 2)] ────► RICE, WSJF, Pareto 80/20: Lọc 20% cốt lõi tạo 80% giá trị
       │
       ▼
[Dự toán & Tiến độ (Trụ cột 1)] ──► Cone of Uncertainty, Hofstadter, CCPM: Tránh bẫy 90-90
       │
       ▼
[Thiết kế Đội ngũ (Trụ cột 4)] ────► Conway's Law, Dunbar, Dual-Track: Tối ưu tải nhận thức
       │
       ▼
[Kiến trúc & Kỹ nghệ (Trụ cột 5)] ─► Gall, Hyrum, Postel, Lehman, Clean Code: Chống thoái hóa
       │
       ▼
[Thực thi & Tối ưu Luồng (Trụ cột 3)] ─► TOC, Little's Law, Kingman Slack Time: Xóa sổ nghẽn
       │
       ▼
[Release & Đo lường (Trụ cột 6)] ──► DORA & SPACE: Đo lường tốc độ, độ ổn định và văn hóa
```

---

## 4. 🗺️ Cây Thư mục & Hệ thống Tài liệu Chuyên sâu

Hệ thống tài liệu hoàn chỉnh gồm 6 phân hệ chuyên biệt:

### ⏳ 1. Phân hệ Thời gian & Ước lượng (`time-estimation/`)
- **[00_overview.md](./time-estimation/00_overview.md)**: Tổng quan phân hệ ước lượng thời gian.
- **[brooks-law.md](./time-estimation/brooks-law.md)**: Định luật Brooks — Bản chất toán học bùng nổ kênh giao tiếp $C = \frac{n(n-1)}{2}$ và chi phí onboarding lính mới.
- **[hofstadter-law.md](./time-estimation/hofstadter-law.md)**: Định luật Hofstadter — Rủi ro Unknown Unknowns, Planning Fallacy và kỹ thuật ước lượng 3 điểm PERT.
- **[parkinsons-law.md](./time-estimation/parkinsons-law.md)**: Định luật Parkinson — Công việc tự phình to lấp đầy thời gian và kỹ thuật Timeboxing.
- **[cone-of-uncertainty.md](./time-estimation/cone-of-uncertainty.md)**: Hình nón Bất định — Biên độ sai lệch $4\times \rightarrow 1\times$ và tái ước lượng lũy tiến.
- **[ninety-ninety-rule.md](./time-estimation/ninety-ninety-rule.md)**: Quy tắc 90-90 — Bẫy 10% chặng cuối chiếm 90% nỗ lực và Definition of Done nhị phân.
- **[student-syndrome.md](./time-estimation/student-syndrome.md)**: Hội chứng Học sinh — Trì hoãn tiêu tán buffer và giải pháp Sprint Buffer tập trung (CCPM).

### 🎯 2. Phân hệ Cân đối Phạm vi & Ưu tiên (`prioritization/`)
- **[00_overview.md](./prioritization/00_overview.md)**: Tổng quan các mô hình ưu tiên backlog.
- **[iron-triangle.md](./prioritization/iron-triangle.md)**: Tam giác Sắt — Đảo ngược vị thế Waterfall vs Agile và tính bất khả xâm phạm của Chất lượng.
- **[rice-scoring.md](./prioritization/rice-scoring.md)**: Khung chấm điểm RICE — Công thức $\frac{R \times I \times C}{E}$ định lượng giá trị kinh doanh.
- **[wsjf-cost-of-delay.md](./prioritization/wsjf-cost-of-delay.md)**: WSJF & Cost of Delay — Tối ưu hóa kinh tế bằng chi phí chậm trễ.
- **[kano-model.md](./prioritization/kano-model.md)**: Mô hình Kano — Phân loại Must-be, Performance, Delighters và thoái hóa kỳ vọng.
- **[pareto-principle.md](./prioritization/pareto-principle.md)**: Nguyên lý Pareto 80/20 — Lọc 20% tính năng cốt lõi và dập tắt 80% vụ crash từ 20% bug gốc rễ.

### 🌊 3. Phân hệ Dòng chảy & Điểm nghẽn (`flow-efficiency/`)
- **[00_overview.md](./flow-efficiency/00_overview.md)**: Tổng quan lý thuyết dòng chảy và quản trị hàng đợi.
- **[theory-of-constraints.md](./flow-efficiency/theory-of-constraints.md)**: Thuyết Điểm nghẽn (TOC) — 5 bước tập trung giải phóng điểm nghẽn của Goldratt.
- **[littles-law-and-wip.md](./flow-efficiency/littles-law-and-wip.md)**: Định luật Little & Giới hạn WIP — Mối quan hệ $\text{Cycle Time} = \frac{\text{WIP}}{\text{Throughput}}$.
- **[lead-time-vs-cycle-time.md](./flow-efficiency/lead-time-vs-cycle-time.md)**: Lead Time vs. Cycle Time — Công thức Flow Efficiency và triệt tiêu $85\%$ thời gian chờ chết.
- **[kingmans-formula.md](./flow-efficiency/kingmans-formula.md)**: Công thức Kingman — Tại sao ép 100% công suất làm thời gian chờ bùng nổ vô tận; nghệ thuật tạo 20% Slack Time.
- **[amdahls-law.md](./flow-efficiency/amdahls-law.md)**: Định luật Amdahl — Giới hạn tăng tốc tối đa của hệ thống và đội ngũ do nút thắt tuần tự quy định.

### 🏛️ 4. Phân hệ Cấu trúc Tổ chức & Bẫy Tâm lý (`organizational-biases/`)
- **[00_overview.md](./organizational-biases/00_overview.md)**: Tổng quan tâm lý học quản trị và cấu trúc tổ chức.
- **[conways-law.md](./organizational-biases/conways-law.md)**: Định luật Conway — Cấu trúc phần mềm sao chép sơ đồ phòng ban và Inverse Conway Maneuver.
- **[goodharts-law.md](./organizational-biases/goodharts-law.md)**: Định luật Goodhart — Bẫy lách luật KPI và kỹ thuật ghép đôi Chỉ số Đối trọng (Counter-Metrics).
- **[sunk-cost-fallacy.md](./organizational-biases/sunk-cost-fallacy.md)**: Ảo tưởng Chi phí Chìm — Quy tắc chi phí quá khứ bằng 0 và văn hóa Kill-Feature.
- **[law-of-triviality.md](./organizational-biases/law-of-triviality.md)**: Định luật Tầm thường (Bike-shedding) — Hiện tượng tranh cãi chuyện vặt và tự động hóa 100% linter/style.
- **[chestertons-fence.md](./organizational-biases/chestertons-fence.md)**: Hàng rào Chesterton — Nguyên tắc bất khả xâm phạm: Hiểu lý do trước khi xóa legacy code.
- **[dunbars-number-cognitive-load.md](./organizational-biases/dunbars-number-cognitive-load.md)**: Số Dunbar & Tải trọng Nhận thức — Giới hạn sinh học 5-8 người (Two-pizza) và 150 người.
- **[peter-principle.md](./organizational-biases/peter-principle.md)**: Nguyên lý Peter — Bẫy thăng chức kỹ sư giỏi thành quản lý tồi và thang Dual-Track Ladder (IC vs EM).

### ⚙️ 5. Phân hệ Kỹ nghệ & Kiến trúc Mã nguồn (`engineering-laws/`)
- **[00_overview.md](./engineering-laws/00_overview.md)**: Tổng quan các định luật cốt lõi trong kỹ nghệ phần mềm.
- **[hyrums-law.md](./engineering-laws/hyrums-law.md)**: Định luật Hyrum — Mọi hành vi quan sát được của API đều trở thành hợp đồng ngầm gây breaking change.
- **[postels-law.md](./engineering-laws/postels-law.md)**: Định luật Postel (Robustness Principle) — Nghiêm khắc khi gửi đi, bao dung khi nhận lại (Tolerant Reader).
- **[lehmans-laws.md](./engineering-laws/lehmans-laws.md)**: Các Định luật Lehman — Phần mềm bắt buộc tiến hóa liên tục và suy thoái chất lượng trừ khi được refactor.
- **[kernighans-law.md](./engineering-laws/kernighans-law.md)**: Định luật Kernighan — Nghịch lý debug code quá thông minh và triết lý Boring Code.
- **[galls-law.md](./engineering-laws/galls-law.md)**: Định luật Gall — Mọi hệ thống phức tạp hiệu quả đều tiến hóa từ hệ thống đơn giản chạy được (MVP & Walking Skeleton).
- **[broken-windows-theory.md](./engineering-laws/broken-windows-theory.md)**: Thuyết Cửa Sổ Vỡ — Cơ chế tâm lý hoại tử codebase và quy tắc Zero-Tolerance đối với code bẩn.

### 📊 6. Phân hệ Đo lường Hiệu năng Kỹ thuật (`engineering-metrics/`)
- **[00_overview.md](./engineering-metrics/00_overview.md)**: Tổng quan đo lường hiệu suất chuyển giao phần mềm.
- **[dora-metrics.md](./engineering-metrics/dora-metrics.md)**: 4 Chỉ số DORA — Deployment Frequency, Lead Time for Changes, Change Failure Rate, Time to Restore Service (MTTR).
- **[space-framework.md](./engineering-metrics/space-framework.md)**: Khung Năng suất Toàn diện SPACE — 5 chiều cân bằng: Satisfaction, Performance, Activity, Communication, Efficiency.

