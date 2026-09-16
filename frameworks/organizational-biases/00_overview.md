---
id: pm-organizational-biases-overview
title: 'Organizational Architecture & Cognitive Biases Overview'
description: 'Tổng quan các quy luật cấu trúc tổ chức, cơ chế lách chỉ số và các bẫy tâm lý sai lầm trong quản trị công nghệ'
tags:
  - project-management
  - organizational-architecture
  - cognitive-biases
  - leadership
  - systems-thinking
scopePaths:
  - docs/agent-knowledge/frameworks/organizational-biases/
related:
  - pm-frameworks-overview
  - pm-conways-law
  - pm-goodharts-law
  - pm-sunk-cost-fallacy
  - pm-law-of-triviality
  - pm-chestertons-fence
  - pm-dunbars-number-cognitive-load
  - pm-peter-principle
---

# 🏛️ Organizational Architecture & Cognitive Biases Overview

<!-- convention-summary-start -->

### Organizational Biases Overview Summary

- **Core Architecture / Purpose**: Domain directory analyzing socio-technical interactions, executive metric gaming, and cognitive traps that derail software architecture.
- **Key Sub-modules & Laws**:
  - [Conway's Law](./conways-law.md): Software architectures mirror organizational communication lines; Inverse Conway Maneuver.
  - [Goodhart's Law](./goodharts-law.md): Corruption of metrics when transformed into targets; paired counter-metrics.
  - [Sunk Cost Fallacy](./sunk-cost-fallacy.md): Irrational commitment to failing architectures; Kill-Switch culture and data-driven pivots.
  - [Law of Triviality (Bike-shedding)](./law-of-triviality.md): Disproportionate focus on trivial matters (PR formatting, button colors) over complex core architecture.
  - [Chesterton's Fence](./chestertons-fence.md): Golden rule of legacy code refactoring — understand why a rule or code snippet was created before deleting it.
  - [Dunbar's Number & Cognitive Load](./dunbars-number-cognitive-load.md): Cognitive thresholds in team sizing (Two-pizza teams, 150-person limit) and domain burden reduction.
  - [The Peter Principle](./peter-principle.md): The incompetence trap in promotions and the vital necessity of Dual-Track Engineering Ladders (IC vs. EM).
- **Scope & Code Paths**: Applied in engineering organization design, performance appraisal reviews, and architectural pivot decisions in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Chiều kích Xã hội - Kỹ thuật (Socio-Technical Systems)

Phần mềm không tồn tại độc lập trong không gian máy tính trừu tượng; phần mềm được viết bởi con người, làm việc trong các tổ chức có thứ bậc, cảm xúc, định kiến và hệ thống động lực khen thưởng/kỷ luật riêng.

Hiểu rõ các quy luật về tổ chức và tâm lý học giúp người làm công nghệ:
- Không ngây thơ tin rằng một kiến trúc hoàn hảo trên giấy có thể vận hành trong một cơ cấu nhân sự rời rạc.
- Tránh việc thiết lập các chỉ số KPI tai hại biến kỹ sư thành những kẻ "lách luật" chuyên nghiệp.
- Dũng cảm cắt bỏ các tính năng hoặc nhánh code thất bại thay vì cố chấp bám đuổi trong vô vọng.

---

## 2. 🗺️ Danh mục Các Quy luật trong Phân hệ này

| Quy luật / Mô hình | Trọng tâm giải quyết | Tài liệu chi tiết |
| :--- | :--- | :--- |
| **Định luật Conway** | Kiến trúc phần mềm luôn sao chép cấu trúc giao tiếp của công ty; áp dụng Thao tác Đảo ngược Conway (*Inverse Conway*) để tái thiết kế team. | [conways-law.md](./conways-law.md) |
| **Định luật Goodhart** | Khi một thước đo bị biến thành mục tiêu ép buộc, nó lập tức bị thao túng; bắt buộc phải ghép đôi các Chỉ số Đối trọng (*Counter-Metrics*). | [goodharts-law.md](./goodharts-law.md) |
| **Ảo tưởng Chi phí Chìm** | Tâm lý tiếc nuối thời gian và tiền bạc đã mất trong quá khứ làm sai lệch quyết định tương lai; văn hóa "Dũng cảm Cắt lỗ" (*Kill-Feature*). | [sunk-cost-fallacy.md](./sunk-cost-fallacy.md) |
| **Định luật Tầm thường (Bike-shedding)** | Xu hướng tranh luận gay gắt những chuyện lặt vặt (màu sắc, tên biến) và lướt qua các vấn đề kỹ thuật hóc búa; giải pháp tự động hóa 100%. | [law-of-triviality.md](./law-of-triviality.md) |
| **Hàng rào Chesterton** | Nguyên tắc bất khả xâm phạm khi dọn dẹp legacy code: Phải hiểu rõ nguyên nhân lịch sử trước khi xóa bỏ bất kỳ dòng code nào. | [chestertons-fence.md](./chestertons-fence.md) |
| **Số Dunbar & Tải trọng Nhận thức** | Giới hạn sinh học não bộ (Two-pizza 5-8 người, Dunbar 150 người) và giải pháp triệt tiêu Extraneous Load cho team. | [dunbars-number-cognitive-load.md](./dunbars-number-cognitive-load.md) |
| **Nguyên lý Peter** | Nghịch lý thăng chức lập trình viên giỏi thành nhà quản lý tồi; thiết kế thang sự nghiệp song song (Dual-Track Ladder). | [peter-principle.md](./peter-principle.md) |
