---
id: pm-ninety-ninety-rule
title: "The Ninety-Ninety Rule: Cargill's Law of Project Completion Traps"
description: "Quy tắc 90-90 của Tom Cargill, ảo tưởng 'sắp xong 90% rồi' và tại sao 10% chặng cuối của dự án lại tốn 90% toàn bộ công sức"
tags:
  - project-management
  - time-estimation
  - ninety-ninety-rule
  - cargills-law
  - estimation
  - definition-of-done
  - release-management
scopePaths:
  - docs/agent-knowledge/frameworks/time-estimation/
related:
  - pm-time-estimation-overview
  - pm-hofstadter-law
  - pm-parkinsons-law
  - pm-cone-of-uncertainty
---

# 🏁 Quy Tắc 90-90 (The Ninety-Ninety Rule)

> *"90% đầu tiên của dòng code chiếm 90% thời gian phát triển dự kiến.*  
> *10% dòng code còn lại chiếm 90% thời gian phát triển còn lại!"*  
> — **Tom Cargill**, Kỹ sư Nghiên cứu tại Bell Labs (được Jon Bentley trích dẫn trong *Communications of the ACM*, 1985).

<!-- convention-summary-start -->

### Ninety-Ninety Rule Summary

- **The Math of the Never-Ending 90%**: $90\% + 90\% = 180\%$ thời gian thực tế so với kế hoạch ban đầu. Khi một lập trình viên hào hứng báo cáo *"Em đã code xong 90% tính năng rồi!"*, thực chất họ mới chỉ hoàn thành được đúng một nửa đoạn đường.
- **The Asymmetry of "Happy Path" vs. "Edge Cases"**: 
  - $90\%$ đầu tiên: Viết luồng chính chạy vui vẻ (Happy Path), logic cơ bản trên môi trường Localhost.
  - $10\%$ còn lại: Xử lý ngoại lệ (Error handling), bảo mật, race conditions, tương thích trình duyệt, test tải, ghi log, CI/CD pipeline, và fix bug trên Production.
- **Actionable Remedy**: Thiết lập **Definition of Done (DoD)** nghiêm ngặt và đo lường tiến độ dựa trên *Tính năng đã chạy được trên Staging* thay vì dựa trên *Phần trăm code dev tự báo cáo*.
<!-- convention-summary-end -->

---

## 1. 🔍 Phân Tích Ảo Tưởng "Sắp Xong Rồi" (Almost Done Syndrome)

```
Thời Gian Thực Tế
┌──────────────────────────────────────────────┬──────────────────────────────────────────────┐
│  GIAI ĐOẠN 1: 90% THỜI GIAN ĐẦU              │  GIAI ĐOẠN 2: 90% THỜI GIAN THỰC             │
│  - Viết 90% code logic chính (Happy Path)    │  - Viết 10% code xử lý ngoại lệ (Edge Cases) │
│  - Mock data trên máy Local                  │  - Fix bug hồi quy (Regression bugs)         │
│  - Dev cảm giác: "Chắc 2 ngày nữa là xong!"  │  - Tối ưu truy vấn DB, gỡ race conditions    │
│                                              │  - Viết tài liệu, deploy lên Staging         │
│                                              │  - Tích hợp cổng thanh toán bên thứ ba       │
└──────────────────────────────────────────────┴──────────────────────────────────────────────┘
 ◄────────────── 50% Nỗ lực Thực ─────────────► ◄────────────── 50% Nỗ lực Thực ─────────────►
```

Tại sao lập trình viên luôn rơi vào bẫy này?
1. **Happy Path Fallacy**: Não bộ con người luôn tự động hình dung kịch bản lý tưởng: mạng luôn có, database không bao giờ rớt, người dùng luôn nhập đúng định dạng.
2. **The Long Tail of Production Readiness**: Đưa một đoạn code "chạy được trên máy dev" tới mức "chạy an toàn trên hệ thống phục vụ hàng triệu người dùng" đòi hỏi hàng trăm bài kiểm tra phụ trợ.

---

## 2. 🛡️ Chiến Lược Dập Tắt Bẫy 90-90

### 1. Áp Dụng Definition of Done (DoD) Không Khoan Nhượng
Một User Story không bao giờ được coi là "xong 90%". Trong Agile, tiến độ là **Nhị phân (Binary: 0% hoặc 100%)**:
- **0%**: Nếu code chưa pass CI, chưa có Unit Test, chưa deploy lên Staging.
- **100%**: Khi và chỉ khi Product Owner đã bấm duyệt và tính năng đã sẵn sàng bật Feature Flag trên Production.

```
┌────────────────────────────────────────────────────────┐
│             DEFINITION OF DONE (DoD) CHECKLIST         │
├────────────────────────────────────────────────────────┤
│ [ ] Code đã qua Code Review (ít nhất 1 Senior duyệt)   │
│ [ ] Unit Tests pass 100% (Line Coverage > 80%)         │
│ [ ] Integration Tests & E2E Tests đã pass trên CI      │
│ [ ] Không phát sinh Security Vulnerabilities           │
│ [ ] Đã cấu hình Metric / Telemetry / Error Alerts      │
│ [ ] Đã deploy thành công lên Staging Environment       │
│ [ ] Product Owner nghiệm thu đúng Acceptance Criteria  │
└────────────────────────────────────────────────────────┘
```

### 2. Phát Triển Theo Lát Cắt Mỏng Dọc (Vertical Slicing)
Thay vì làm 90% toàn bộ giao diện rồi mới chuyển sang làm Backend (Horizontal Slicing):
- Hãy cắt bài toán thành từng **lát cắt dọc siêu mỏng** (Ví dụ: Chỉ hoàn thành luồng "Đăng nhập bằng Email" từ UI -> DB -> Email Service xong trọn vẹn 100%).
- Điều này loại bỏ hoàn toàn giai đoạn "nghẽn tích hợp" ở cuối dự án.
