---
id: pm-prioritization-overview
title: 'Scope Balancing & Prioritization Frameworks Overview'
description: 'Tổng quan các mô hình định lượng giá trị, cân đối phạm vi và thiết lập thứ tự ưu tiên trong phát triển phần mềm'
tags:
  - project-management
  - prioritization
  - scope-management
  - decision-making
  - product-management
scopePaths:
  - docs/agent-knowledge/frameworks/prioritization/
related:
  - pm-frameworks-overview
  - pm-iron-triangle
  - pm-rice-scoring
  - pm-wsjf-cost-of-delay
  - pm-kano-model
  - pm-pareto-principle
---

# 🎯 Scope Balancing & Prioritization Frameworks Overview

<!-- convention-summary-start -->

### Prioritization Frameworks Overview Summary

- **Core Architecture / Purpose**: Domain directory of quantitative prioritization and trade-off mechanics eliminating emotional bias from product and engineering backlogs.
- **Key Sub-modules & Models**:
  - [The Iron Triangle](./iron-triangle.md): Scope vs. Time vs. Cost dynamics and Agile fixed-cadence inversion.
  - [RICE Scoring](./rice-scoring.md): Standardized scoring matrix combining Reach, Impact, Confidence, and Effort.
  - [WSJF & Cost of Delay](./wsjf-cost-of-delay.md): Economic optimization formula prioritizing high-urgency, short-duration tasks.
  - [Kano Model](./kano-model.md): Feature classification into Must-be, Performance, and Delighters with expectation decay.
  - [The Pareto Principle (80/20 Rule)](./pareto-principle.md): Power-law distribution in software features, bug crashing patterns, and performance optimization.
- **Scope & Code Paths**: Applied in backlog grooming, roadmap planning, and feature trade-offs in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Tại sao Cần Khung Định lượng Ưu tiên?

Trong mọi dự án phần mềm, số lượng ý tưởng và yêu cầu từ các bên liên quan (Product, Sales, Marketing, Người dùng, Kỹ thuật) luôn vượt gấp $5\times$ đến $10\times$ năng lực sản xuất thực tế của đội ngũ.

Nếu không có một khung định lượng minh bạch:
- Thứ tự ưu tiên sẽ bị chi phối bởi cảm tính hoặc tiếng nói của người có chức danh cao nhất trong phòng họp (HiPPO - *Highest Paid Person's Opinion*).
- Đội ngũ rơi vào trạng thái "cái gì cũng khẩn cấp", dẫn đến việc ôm đồm, phân tán nguồn lực và không hoàn thành được mục tiêu cốt lõi nào.

---

## 2. 🗺️ Danh mục Các Mô hình trong Phân hệ này

| Mô hình / Khung | Trọng tâm giải quyết | Tài liệu chi tiết |
| :--- | :--- | :--- |
| **Tam giác Sắt (The Iron Triangle)** | Cân đối mối quan hệ ràng buộc giữa Phạm vi (Scope), Thời gian (Time) và Chi phí (Cost) với Chất lượng ở trung tâm. | [iron-triangle.md](./iron-triangle.md) |
| **Khung Chấm điểm RICE** | Định lượng điểm số ưu tiên qua 4 yếu tố: Reach (Độ phủ), Impact (Tác động), Confidence (Độ tin cậy) và Effort (Công sức). | [rice-scoring.md](./rice-scoring.md) |
| **WSJF & Cost of Delay** | Tối ưu hóa kinh tế bằng cách đo lường tổn thất khi ra mắt muộn và chia cho độ dài tác vụ (Weighted Shortest Job First). | [wsjf-cost-of-delay.md](./wsjf-cost-of-delay.md) |
| **Mô hình Kano** | Phân tích kỳ vọng và cảm xúc người dùng thành 3 tầng: Bắt buộc (Must-be), Tỷ lệ thuận (Performance) và Bất ngờ (Delighters). | [kano-model.md](./kano-model.md) |
| **Nguyên lý Pareto (80/20)** | Lọc ra 20% tính năng cốt lõi tạo ra 80% giá trị; tập trung xử lý 20% bug gốc rễ dập tắt 80% vụ sập hệ thống. | [pareto-principle.md](./pareto-principle.md) |
