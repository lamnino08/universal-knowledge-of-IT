---
id: pm-engineering-laws-overview
title: 'Engineering & Software Architecture Laws Overview'
description: 'Tổng quan các định luật kinh điển trong kỹ nghệ phần mềm, thiết kế API, tiến hóa hệ thống và tư duy kiến trúc'
tags:
  - project-management
  - software-engineering
  - system-architecture
  - engineering-laws
  - api-design
  - code-quality
scopePaths:
  - docs/agent-knowledge/frameworks/engineering-laws/
related:
  - pm-frameworks-overview
  - pm-hyrums-law
  - pm-postels-law
  - pm-lehmans-laws
  - pm-kernighans-law
  - pm-galls-law
  - pm-broken-windows-theory
---

# ⚙️ Engineering & Architecture Laws Overview

<!-- convention-summary-start -->

### Engineering Laws Overview Summary

- **Core Architecture / Purpose**: Comprehensive guide to fundamental empirical laws governing software design, API contracts, system evolution, cognitive debugging traps, and codebase entropy.
- **Key Sub-modules & Laws**:
  - [Hyrum's Law](./hyrums-law.md): Implicit contracts & why every observable API behavior will be relied upon.
  - [Postel's Law](./postels-law.md): Robustness principle (conservative in what you do, liberal in what you accept).
  - [Lehman's Laws of Software Evolution](./lehmans-laws.md): Continuous change, increasing complexity, and conservation of familiarity.
  - [Kernighan's Law](./kernighans-law.md): The clever code paradox and debugging limits.
  - [Gall's Law](./galls-law.md): Complex systems evolving from working simple systems vs. top-down design failures.
  - [Broken Windows Theory](./broken-windows-theory.md): Codebase rot, technical debt escalation, and the Boy Scout rule.
- **Scope & Code Paths**: Applied across API versioning, system architecture, refactoring protocols, and engineering standards in `docs/project-management/`.
<!-- convention-summary-end -->

---

## 1. 🎯 Tại sao Kỹ sư Cần Nắm vững các Định luật Kỹ nghệ Phần mềm?

Nếu các mô hình quản lý dự án giúp chúng ta trả lời câu hỏi *"Khi nào release và làm tính năng gì?"*, thì **các định luật Kỹ nghệ Phần mềm (Engineering Laws)** giúp chúng ta trả lời câu hỏi sống còn: **"Tại sao mã nguồn và hệ thống lại suy thoái theo thời gian, và làm sao để xây dựng một kiến trúc bền bỉ qua năm tháng?"**.

Các định luật này không phải là lý thuyết hàn lâm, mà là kết quả đúc rút từ hàng thập kỷ va vấp của các kỹ sư huyền thoại tại Bell Labs, Google, IETF, và các dự án mã nguồn mở toàn cầu.

---

## 2. 🗺️ Danh mục Các Định luật trong Phân hệ này

| Định luật / Nguyên lý | Tác giả & Bối cảnh | Bản chất cốt lõi | Tài liệu chi tiết |
| :--- | :--- | :--- | :--- |
| **Hyrum's Law** | Hyrum Wright (Google) | Khi có đủ người dùng, mọi hành vi quan sát được của API (kể cả thứ tự trả về, tốc độ, side-effect) đều trở thành hợp đồng ngầm phá vỡ tương thích khi thay đổi. | [hyrums-law.md](./hyrums-law.md) |
| **Postel's Law (Robustness Principle)** | Jon Postel (IETF RFC 760) | "Hãy nghiêm khắc với những gì bạn gửi đi, và hãy bao dung/mềm dẻo với những gì bạn tiếp nhận" trong thiết kế giao thức mạng và API. | [postels-law.md](./postels-law.md) |
| **Lehman's Laws of Software Evolution** | Meir Lehman (IBM/Imperial College) | Phần mềm bắt buộc phải liên tục thay đổi nếu không muốn trở nên vô dụng; và độ phức tạp sẽ tăng vô hạn trừ khi có nỗ lực refactor chủ động. | [lehmans-laws.md](./lehmans-laws.md) |
| **Kernighan's Law** | Brian Kernighan (Unix/C Co-creator) | "Debugging khó gấp đôi viết code. Nếu bạn viết code thông minh/phức tạp hết mức có thể, bạn sẽ không đủ thông minh để debug nó." | [kernighans-law.md](./kernighans-law.md) |
| **Gall's Law** | John Gall (Systemantics) | Mọi hệ thống phức tạp chạy được đều bắt nguồn từ một hệ thống đơn giản chạy được trước đó. Một hệ thống phức tạp được thiết kế từ con số 0 sẽ luôn thất bại. | [galls-law.md](./galls-law.md) |
| **Broken Windows Theory** | Wilson & Kelling / Hunt & Thomas | Một đoạn code bẩn, một bài test bị disable không được sửa chữa sẽ tạo ra tiền lệ tâm lý khiến toàn bộ codebase bị hoại tử nhanh chóng. | [broken-windows-theory.md](./broken-windows-theory.md) |
