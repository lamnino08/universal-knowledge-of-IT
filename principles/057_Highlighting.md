---
name: "Highlighting"
vi: "Kỹ thuật làm nổi bật (Highlighting)"
summary: "Highlighting (Kỹ thuật làm nổi bật (Highlighting)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Highlighting (Kỹ thuật làm nổi bật (Highlighting))

> **Tóm tắt cốt lõi (Summary)**: Highlighting là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Highlighting
A technique for bringing attention to an area of text or image.
Highlighting is an effective technique for bringing attention to elements of a design.
If applied improperly, however, highlighting can be ineffective, and actually reduce
performance in these areas. The following guidelines address the benefits and
liabilities of common highlighting techniques.1
General
Highlight no more than 10 percent of the visible design; highlighting effects
are diluted as the percentage increases. Use a small number of highlighting
tech-niques applied consistently throughout the design.
Bold, Italics, and Underlining
Use bold, italics, and underlining for titles, labels, captions, and short word
sequences when the elements need to be subtly differentiated. Bolding is
generally preferred over other techniques as it adds minimal noise to the design
and clearly highlights target elements. Italics add minimal noise to a design,
but are less detectable and legible. Underlining adds considerable noise and
compromises legibility, and should be used sparingly if at all.2
Typeface
Uppercase text in short word sequences is easily scanned, and thus can be
advantageous when applied to labels and keywords within a busy display. Avoid
using different fonts as a highlighting technique. A detectable difference between
fonts is difficult to achieve without also disrupting the aesthetics of the typography.
Color
Color is a potentially effective highlighting technique, but should be used sparingly
and only in concert with other highlighting techniques. Highlight using a few
desaturated colors that are clearly distinct from one another.
Inversing
Inversing elements works well with text, but may not work as well with icons or
shapes. It is effective at attracting attention, but adds considerable noise to the
design and therefore should be used sparingly.
Blinking
Blinking—flashing an element between two states—is a powerful technique
for attracting attention. Blinking should be used only to indicate highly critical
information that requires an immediate response, such as an emergency status
light. It is important to be able to turn off the blinking once it is acknowledged,
as it compromises legibility, and distracts from other tasks.
See also Color, Legibility, and Readability.

1 See, for example, “A Review of Human Factors
Guidelines and Techniques for the Design of
Graphical Human-Computer Interfaces” by
Martin Maguire, International Journal of Man-
Machine Studies, 1982, vol. 16(3), p. 237–261.
2 A concise summary of typographic principles
of this kind is found in The Mac is Not a
Typewriter by Robin Williams, Peachpit Press,
1990. Despite the title, the book is of value to
non-Macintosh owners as well.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

beginning
little irritated
very short
you
very
you
Highlighting 127
General
“You mean you can’t take less,” said the Hatter, “it’s very
easy to take more than nothing.”
“Nobody asked your opinion,” said Alice.
“You mean you can’t take less,” said the Hatter, “it’s very
easy to take more than nothing.”
“Nobody asked your opinion,” said Alice.
Typeface
“What is a Caucus-race?” said Alice; not that she wanted
much to know, but the Dodo had paused as if it thought that
somebody ought to speak, and no one else seemed
inclined to say anything.
“What IS a Caucus-race?” said Alice; not that she wanted
much to know, but the Dodo had paused as if it thought that
SOMEBODY ought to speak, and no one else seemed
inclined to say anything.
Bold, Italics, and Underlining
“I can’t explain myself, I’m afraid, sir”
said Alice, “because I’m not myself,
you see.”
Advice from a Caterpillar 	Advice from a Caterpillar 	Advice from a Caterpillar
“I can’t explain myself, I’m afraid, sir”
said Alice, “because I’m not myself,
you see.”
“I can’t explain myself, I’m afraid, sir”
said Alice, “because I’m not myself,
you see.”
Who stole the tarts?
Inversing
Color
Which brought them back again to the 	of the
conversation. Alice felt a 	at the Caterpillar’s
making such 	remarks, and she drew herself up
and said, very gravely, “I think, you ought to tell me who
are, first.”
Which brought them back again to the beginning of the
conversation. Alice felt a little irritated at the Caterpillar’s
making such 	short remarks, and she drew herself up
and said, very gravely, “I think, you ought to tell me who
are, first.”
Who stole the tarts?

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Highlighting** vào thiết kế giao diện web/mobile:
1. **Phù hợp với mục tiêu người dùng**: Đảm bảo thành phần giao diện phục vụ đúng nhóm nhu cầu cốt lõi, tránh gây quá tải nhận thức hoặc tạo rào cản thao tác không cần thiết.
2. **Tuân thủ hệ thống Design Tokens**: Sử dụng màu sắc semantic (`bg-background`, `bg-card`, `text-primary`, `border-border`), khoảng cách breathing whitespace chuẩn mực (`gap-4`, `p-6`), và kiểu chữ rõ ràng (`text-sm`, `text-base`, `font-medium`).
3. **Độ phản hồi & Trạng thái tương tác**: Mọi thành phần tương tác phải có đầy đủ trạng thái Default, Hover, Active, Focus-visible và Disabled rõ ràng.
4. **Khả năng tiếp cận (Accessibility)**: Tuân thủ độ tương phản WCAG 2.1 AA (>= 4.5:1), kích thước tương tác >= 44x44px trên thiết bị di động, và cung cấp thẻ ARIA / text thay thế đầy đủ.

---

## 3. 🛠️ Practical Application (How to Apply)

- **Cấu trúc & Bố cục (Layout & Hierarchy)**: Sắp xếp các thành phần quan trọng ở vị trí ưu tiên tự nhiên theo thị giác (Gutenberg Diagram hoặc Z-pattern), nhóm các thông tin liên quan lại gần nhau.
- **Tương tác & Phản hồi (Interaction & Feedback)**: Cung cấp phản hồi tức thì cho mọi hành động người dùng (loading skeleton, toast notifications, confirmation dialogs khi thao tác nguy hiểm).
- **Tránh dư thừa (Minimalism & Cognitive Ease)**: Loại bỏ các chi tiết thừa thãi, chỉ hiển thị thông tin thực sự cần thiết tại mỗi bước trải nghiệm (áp dụng Progressive Disclosure khi cần).

---

## 4. 🚫 Anti-patterns & Common Pitfalls

- **Overcomplication**: Nhồi nhét quá nhiều thông tin hoặc hiệu ứng không liên quan gây phân tán sự chú ý của người dùng.
- **Thiếu nhất quán**: Sử dụng phong cách trực quan, màu sắc hoặc thuật ngữ bất đồng bộ giữa các trang trong cùng một hệ thống.
- **Bỏ qua phản hồi lỗi**: Không giải thích nguyên nhân lỗi rõ ràng hoặc không có cơ chế hoàn tác (Undo/Forgiveness) cho người dùng.

---

## 5. 💡 Key Takeaway for the Agent

> *"Áp dụng nguyên lý Highlighting để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Color, Legibility, and Readability
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
