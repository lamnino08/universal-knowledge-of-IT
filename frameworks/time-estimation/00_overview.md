---
id: pm-time-estimation-overview
title: 'Time & Estimation Frameworks Overview'
description: 'Tổng quan các quy luật và hiện tượng tâm lý ảnh hưởng đến việc ước lượng thời gian và tiến độ phần mềm'
tags:
  - project-management
  - time-estimation
  - estimation
  - planning
  - scheduling
scopePaths:
  - docs/agent-knowledge/frameworks/time-estimation/
related:
  - pm-frameworks-overview
  - pm-brooks-law
  - pm-hofstadter-law
  - pm-parkinsons-law
  - pm-cone-of-uncertainty
  - pm-ninety-ninety-rule
  - pm-student-syndrome
---

# ⏳ Time & Estimation Frameworks Overview

<!-- convention-summary-start -->

### Time & Estimation Overview Summary

- **Core Architecture / Purpose**: High-level domain overview covering mathematical laws, psychological biases, and uncertainty models in software timeline estimation.
- **Key Sub-modules & Laws**:
  - [Brooks' Law](./brooks-law.md): Communication channel explosion and team ramp-up penalty.
  - [Hofstadter's Law](./hofstadter-law.md): Recursive complexity, unknown unknowns, and PERT 3-point estimation.
  - [Parkinson's Law](./parkinsons-law.md): Work expansion to fill duration and timeboxing mitigation.
  - [Cone of Uncertainty](./cone-of-uncertainty.md): 4x initial estimation variance narrowing across development phases.
  - [The Ninety-Ninety Rule](./ninety-ninety-rule.md): Cargill's Law on the long tail of edge cases and the "90% done" illusion.
  - [Student Syndrome](./student-syndrome.md): Procrastination of individual safety buffers and Centralized Project Buffers (CCPM).
- **Scope & Code Paths**: Applied across sprint grooming, milestone commitments, and resource allocation in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Thách thức Cốt lõi của Ước lượng Phần mềm

Ước lượng thời gian (Estimation) luôn là một trong những bài toán khó nhất của kỹ thuật phần mềm. Khác với xây cầu hay làm đường vốn có vật liệu và quy trình vật lý định sẵn, phần mềm là một sản phẩm thuần túy phi vật thể, nơi mỗi tính năng mới thường là một tác vụ chưa từng được thực hiện trước đó trong ngữ cảnh cụ thể của hệ thống.

Hiểu rõ các quy luật về thời gian giúp đội ngũ:
- Không rơi vào bẫy hứa hẹn phi thực tế với các bên liên quan (Stakeholders).
- Hiểu được tại sao việc tăng nhân sự vào phút chót là một hành động tự sát về tiến độ.
- Thiết lập cơ chế khóa thời gian (Timebox) và quản lý dung sai một cách khoa học.

---

## 2. 🗺️ Danh mục Các Quy luật trong Phân hệ này

| Quy luật / Mô hình | Bản chất cốt lõi | Tài liệu chi tiết |
| :--- | :--- | :--- |
| **Định luật Brooks** | Thêm người vào dự án đang trễ hạn chỉ làm dự án trễ hơn nữa do bùng nổ kênh giao tiếp $C = \frac{n(n-1)}{2}$. | [brooks-law.md](./brooks-law.md) |
| **Định luật Hofstadter** | Dự án luôn tốn nhiều thời gian hơn dự tính do rủi ro ẩn (Unknown Unknowns) và bẫy Planning Fallacy. | [hofstadter-law.md](./hofstadter-law.md) |
| **Định luật Parkinson** | Công việc luôn tự phình to để lấp đầy thời gian được giao (mạ vàng tính năng, tối ưu hóa sớm). | [parkinsons-law.md](./parkinsons-law.md) |
| **Hình nón Bất định** | Sai số ước lượng ở giai đoạn đầu có thể lên tới $4\times$ và chỉ tiệm cận $1\times$ khi code đã chạy. | [cone-of-uncertainty.md](./cone-of-uncertainty.md) |
| **Quy tắc 90-90 (Cargill)** | 10% chặng cuối chiếm 90% nỗ lực thực tế; áp dụng Definition of Done để chống bẫy "sắp xong". | [ninety-ninety-rule.md](./ninety-ninety-rule.md) |
| **Hội chứng Học sinh** | Tâm lý ỷ lại đốt cháy thời gian an toàn; giải pháp gom đệm an toàn tập trung (CCPM). | [student-syndrome.md](./student-syndrome.md) |
