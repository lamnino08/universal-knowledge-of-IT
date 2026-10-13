# VisualSelect Component Usage & Zero-Forced Input Pattern

**Category:** ui-ux
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-12

## 🔍 Problem / Context
Các nút chọn dạng lưới (Option Grid) trong Modal bị mất chữ do lỗi tương phản màu (white-on-white) và bị gán cứng giá trị mặc định khiến người dùng bị ép buộc chọn khi không có nhu cầu.

## 💡 Solution & Implementation
1. Bắt buộc dùng component chuẩn `VisualSelect` (variant='card' hoặc 'pill') thay vì tự chế thẻ button. VisualSelect tự động quản lý semantic tokens (`border-text-primary`, `bg-card`, `text-text-primary`), animation spring indicator và độ tương phản WCAG 2.1 AA.
2. Với các trường tùy chọn (optional) như tình trạng hàng hóa/game, áp dụng pattern Toggle Deselect `if (oldVal === newVal) setField(null)` và không set option default để đảm bảo nguyên tắc Zero-Forced Input.

## ⚠️ Anti-Patterns / Pitfalls
Tự chế lưới <button> thủ công với class `bg-primary text-white` hoặc ép cứng option mặc định cho các trường tùy chọn (optional) trong Modal. Khi chạy trên Dark Theme, biến --primary sáng màu làm chữ trắng bị chói lóa, mất tương phản và vi phạm chuẩn WCAG AA.

## 📂 Related Files
- `workspace/web/components/form/base-component/select/VisualSelect.tsx`
- `workspace/web/components/boardgame/collection/GameCollectionDetailModal.tsx`
- `docs/frontend/components/form-controls/select-dropdowns.md`

