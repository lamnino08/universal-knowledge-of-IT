# Host Social Connection & Realtime Interaction 3-Phase Model Roadmap

**Category:** architecture
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-04

## 🔍 Problem / Context
Thiết kế cơ chế giao tiếp và kết nối xã hội (Social Connection) tối ưu cho các buổi Host Session (Boardgame, Badminton) thay vì nhúng khung bình luận tĩnh không phù hợp.

## 💡 Solution & Implementation
Triển khai Mô hình kết nối 3 giai đoạn (3-Phase Connection Model): 1. Pre-Join: Public Q&A Card + Social Icebreaker (gu chơi); 2. In-Session: Session Group Chat qua WebSocket (chỉ mở cho JOINED participants để check-in, gửi ảnh, tin nhắn mẫu); 3. Post-Session: Endorsement & Karma Feedback Loop kèm 1-Click Add Friend sau khi session COMPLETED. Đã lưu chi tiết task roadmap tại docs/frontend/features/host/host_social_connection_roadmap.md.

## ⚠️ Anti-Patterns / Pitfalls
Không dùng CommentList thông thường (dạng bình luận tĩnh dài hạn của Blog/Movie) cho các buổi Host Session vì đây là sự kiện thực tế có thời gian ngắn, cần phản hồi thời gian thực và dễ gây loãng giao diện.

## 📂 Related Files
- `docs/frontend/features/host/host_social_connection_roadmap.md`
- `workspace/web/components/host/`

