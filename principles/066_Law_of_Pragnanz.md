---
name: "Law of Prägnanz"
vi: "Định luật đơn giản hóa Prägnanz"
summary: "Law of Prägnanz (Định luật đơn giản hóa Prägnanz): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Law of Prägnanz (Định luật đơn giản hóa Prägnanz)

> **Tóm tắt cốt lõi (Summary)**: Law of Prägnanz là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Law of Prägnanz
A tendency to interpret ambiguous images as simple and
complete, versus complex and incomplete.1
The Law of Prägnanz is one of several principles referred to as Gestalt principles
of perception. It asserts that when people are presented with a set of ambiguous
elements (elements that can be interpreted in different ways), they interpret the
elements in the simplest way. Here, “simplest” refers to arrangements having
fewer rather than more elements, having symmetrical rather than asymmetrical
compositions, and generally observing the other Gestalt principles of perception.2
For example, a set of shapes that touches at their edges could be interpreted
as either adjacent or overlapping. When the shapes are complex, the simplest
interpretation is that they are adjacent like pieces in a puzzle. When the shapes
are simple, the simplest interpretation is that they overlap one another. The
law applies similarly to the way in which images are recalled from memory. For
example, people recall the positions of countries on maps as more aligned and
symmetrical than they actually are.
The tendency to perceive and recall images as simply as possible indicates that
cognitive resources are being applied to translate or encode images into simpler
forms. This suggests that fewer cognitive resources may be needed if images are
simpler at the outset. Research supports this idea and confirms that people are
better able to visually process and remember simple figures than complex figures.3
Therefore, minimize the number of elements in a design. Note that symmetrical
compositions are perceived as simpler and more stable than asymmetrical
compositions, but symmetrical compositions are also perceived to be less
interesting. Favor symmetrical compositions when efficiency of use is the priority,
and asymmetrical compositions when interestingness is the priority. Consider
all of the Gestalt principles of perception (closure, common fate, figure-ground
relationship, good continuation, proximity, similarity, and uniform connectedness).
See also Aesthetic-Usability Effect, Ockham’s Razor, Rule of Thirds, and
Visuospacial Resonance.

1 Also known as the law of good configuration,
law of simplicity, law of pregnance, law of
precision, and law of good figure.
2 The seminal work on the Law of Prägnanz
is Principles of Gestalt Psychology by Kurt
Koffka, Harcourt Brace, 1935.
3 See, for example, “The Status of Minimum
Principle in the Theoretical Analysis of Visual
Perception” by Gary Hatfield and William
Epstein, Psychological Bulletin, 1985, vol. 97,
p. 155–186.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Law of Prägnanz 145
Low resolution images (left) of a
rock formation on Mars led many
to conclude that intelligent life once
existed there. Higher-resolution
images (right) taken some years
later suggest a more Earth-based
explanation: Humans tend to add
order and meaning to patterns and
formations that do not exist outside
their perception.
Both sets of figures are interpreted
as simple overlapping shapes, rather
than a more complex interpretation—
e.g., two inverted “L” shapes and a
square, and two triangles and a five-
sided polygon.
These sets of characters are
interpreted as single faces rather than
multiple independent characters.
Dazzle camouflage schemes used on
war ships were designed to prevent
simple interpretations of boat type and
orientation, making it a difficult target
for submarines. This is a rendering of
the French cruiser Gloire.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Law of Prägnanz** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Law of Prägnanz để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Aesthetic-Usability Effect, Ockham’s Razor, Rule of Thirds, and
Visuospacial Resonance
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
