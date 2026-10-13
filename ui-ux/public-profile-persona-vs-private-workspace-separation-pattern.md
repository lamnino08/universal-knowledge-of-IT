# Public Profile Persona vs Private Workspace Separation Pattern

**Category:** ui-ux
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-13

## 🔍 Problem / Context
Khi người dùng A truy cập trang cá nhân công khai của người dùng B (/social/members/[user_slug]), giao diện hiển thị các tab Bookmark/Saved và Lịch sử xem (History), nhưng các component này lại truy vấn dữ liệu riêng tư của người dùng A (người đang đăng nhập) thay vì của người dùng B, gây rò rỉ ngữ cảnh, làm sai lệch mô hình tâm trí và hiển thị trống vô nghĩa. Đồng thời, tài sản xã hội quan trọng nhất là Tủ game (Collection) lại bị giấu đi đối với người ngoài.

## 💡 Solution & Implementation
1. Mở rộng API GET /boardgame/collection hỗ trợ query user_id/user_slug với optionalAuth để cho phép truy vấn tủ game công khai. 2. Frontend phân định rạch ròi isOwner: nếu là người khác xem, ẩn triệt để các tab riêng tư (Saved, History), chỉ mở Tủ game của thành viên ở chế độ View-Only (ẩn nút sửa/xóa/đồng bộ). 3. Bổ sung i18n empty state hướng về người thứ ba ('[Tên] chưa thêm tựa game nào vào tủ nè!') thay vì văn phong kêu gọi chính chủ lưu game.

