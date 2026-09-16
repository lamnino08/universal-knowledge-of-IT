---
id: pm-engineering-metrics-overview
title: 'Engineering Value Delivery Telemetry Overview'
description: 'Tổng quan các hệ thống đo lường hiệu năng chuyển giao phần mềm và năng suất kỹ sư hiện đại'
tags:
  - project-management
  - engineering-metrics
  - telemetry
  - productivity
  - devops
scopePaths:
  - docs/agent-knowledge/frameworks/engineering-metrics/
related:
  - pm-frameworks-overview
  - pm-dora-metrics
  - pm-space-framework
  - telemetry-conventions
---

# 📊 Engineering Value Delivery Telemetry Overview

<!-- convention-summary-start -->

### Engineering Metrics Overview Summary

- **Core Architecture / Purpose**: Domain directory of empirical, outcome-oriented delivery performance and developer productivity frameworks.
- **Key Sub-modules & Frameworks**:
  - [DORA Metrics](./dora-metrics.md): The 4 gold-standard delivery metrics (Deployment Frequency, Lead Time, CFR, MTTR) debunking the speed vs. stability myth.
  - [SPACE Framework](./space-framework.md): Multidimensional productivity model balancing Satisfaction, Performance, Activity, Communication, and Efficiency.
- **Scope & Code Paths**: Applied in automated CI/CD pipeline telemetry, git commit analytics, and developer experience (DX) surveys in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Tại sao Cần Đo lường Bằng Kết quả Thực tế (Outcomes over Output)?

Nhiều tổ chức công nghệ vẫn đo lường năng suất lập trình viên bằng các chỉ số phù phiếm (Vanity Metrics): đếm số commit, đếm số dòng code, hoặc đếm số giờ ngồi trước màn hình. Những chỉ số này không phản ánh giá trị kinh doanh, dễ bị thao túng (theo *Định luật Goodhart*) và làm suy sụp tinh thần kỹ sư.

Hệ thống đo lường hiện đại chuyển dịch hoàn toàn sang **Đo lường Năng lực Chuyển giao Giá trị (Value Delivery Performance)**:
- Hệ thống có khả năng xuất xưởng tính năng nhỏ an toàn hàng ngày không?
- Khi có sự cố xảy ra, mất bao lâu để hệ thống tự phục hồi?
- Kỹ sư có cảm thấy hạnh phúc và có đủ thời gian tập trung sâu (*Deep Work*) không?

---

## 2. 🗺️ Danh mục Các Khung Đo lường trong Phân hệ này

| Khung / Hệ chỉ số | Trọng tâm giải quyết | Tài liệu chi tiết |
| :--- | :--- | :--- |
| **4 Chỉ số Vàng DORA** | Chuẩn mực vàng toàn cầu đo lường tốc độ và độ tin cậy của chuỗi CI/CD (Deployment Frequency, Lead Time, CFR, MTTR). | [dora-metrics.md](./dora-metrics.md) |
| **Khung Năng suất SPACE** | Mô hình 5 chiều toàn diện ngăn chặn kiệt sức: Satisfaction, Performance, Activity, Communication và Efficiency & Flow. | [space-framework.md](./space-framework.md) |
