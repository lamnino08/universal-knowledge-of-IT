---
name: "i18n Copy"
vi: "Copy đa ngôn ngữ (i18n Copy)"
summary: "Viết tiếng Việt và English như hai bản địa hóa tự nhiên, giữ cùng ý định và cảm xúc thay vì dịch từng chữ."
categories:
  - i18n
  - localization
  - writing
---

# Writing Principle: i18n Copy (Copy đa ngôn ngữ)

> **Tóm tắt cốt lõi (Summary)**: Ineffable dùng `vi` làm locale mặc định và có `en` song song. Hai bản cần cùng thông điệp nhưng được viết theo nhịp và cách nói tự nhiên của từng ngôn ngữ.

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Convention i18n của project yêu cầu key dùng `snake_case`, dictionary `vi` và `en` đầy đủ, và locale fallback về `vi`. Đây là quy tắc kỹ thuật; với marketing copy, nguyên tắc tương ứng là giữ ý định, audience và CTA nhất quán giữa các locale.

## 2. 🤖 Agent Instructions for Writing

1. Mặc định viết tiếng Việt nếu người dùng không chỉ định locale.
2. Không dịch từng chữ các câu thân mật, joke, hook hoặc idiom.
3. Giữ tên tính năng/brand term chính xác; bản social có thể diễn giải thêm nhưng không đổi nghĩa.
4. Khi tạo `vi/en`, tạo hai bản độc lập rồi kiểm tra cùng core idea, cảm xúc và CTA.
5. Nếu câu chứa biến động như tên phim, tên người hoặc số lượng, giữ placeholder rõ ràng.

## 3. 🛠️ Practical Application (How to Apply)

| Product term | Vietnamese copy | English copy |
| :--- | :--- | :--- |
| Watch Party | Xem Chung / Mở Rạp Xem Chung | Watch Party |
| Host Sessions | Ghép Kèo | Host Sessions |
| Community | Cộng đồng | Community |
| Watch Now | Xem ngay / Vào xem liền | Watch now |
| Coming soon | Sắp có | Coming soon |

English không nhất thiết phải giữ các câu như “cấm ghost nha!”; hãy viết câu tương đương tự nhiên cho audience English.

## 4. 🚫 Anti-patterns & Common Pitfalls

- Dịch “Xem Chung” thành một cụm máy móc không ai nói.
- Trộn Việt–Anh ngẫu nhiên chỉ vì nghe marketing hơn.
- Viết tiếng Anh dài hơn nhiều và làm lệch promise của bản Việt.
- Đưa key i18n hoặc dot-notation vào caption người dùng.

## 5. 💡 Key Takeaway for the Agent

> *"Cùng một ý định, không nhất thiết cùng một câu."*

## 6. 🔗 See Also & References

- `docs/shared/i18n/README.md`
- `docs/shared/i18n/keys.md`
- Liên quan: Voice and Tone, Platform Adaptation, Product Vocabulary.
