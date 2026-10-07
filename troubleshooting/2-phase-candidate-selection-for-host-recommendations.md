# 2-Phase Candidate Selection for Host Recommendations

**Category:** troubleshooting
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-10-07

## 🔍 Problem / Context
Khi số lượng bài đăng bàn chơi ghép kèo (Host Sessions) trong database tăng lên hàng nghìn bản ghi, việc quét toàn bộ database để chấm điểm và gợi ý sẽ gây nghẽn I/O và lãng phí tài nguyên máy chủ.

## 💡 Solution & Implementation
Áp dụng mô hình 2-Phase Candidate Selection: Phase 1 dùng MySQL Index lọc thô 2 luồng song song với LIMIT 15 (Local Province + Broader Open) khống chế tập ứng viên <= 30 bản ghi; Phase 2 chấm điểm trọng số 4 tiêu chí (Vị trí 35đ, Game 35đ, Lịch 15đ, Tín nhiệm 15đ) trong RAM < 2ms và lấy Top 3.

