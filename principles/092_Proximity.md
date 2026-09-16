---
name: "Proximity"
vi: "Nguyên lý tiệm cận (Proximity)"
summary: "Proximity (Nguyên lý tiệm cận (Proximity)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Proximity (Nguyên lý tiệm cận (Proximity))

> **Tóm tắt cốt lõi (Summary)**: Proximity là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Proximity
Elements that are close together are perceived to be more
related than elements that are farther apart.
The principle of proximity is one of several principles referred to as Gestalt
principles of perception. It asserts that elements close together are perceived as a
single group or chunk, and are interpreted as being more related than elements
that are farther apart. For example, a simple matrix of dots can be interpreted as
consisting of multiple rows, multiple columns, or as a uniform matrix, depending
on the relative horizontal and vertical proximities of the dots.1
The grouping resulting from proximity reduces the complexity of designs and
reinforces the relatedness of the elements. Conversely, a lack of proximity results
in the perception of multiple, disparate chunks, and reinforces differences among
elements. Certain proximal layouts imply specific kinds of relationships, and should
be considered in layout design. For example, connecting or overlapping elements
are commonly interpreted as sharing one or more common attributes, whereas
proximal but non-contacting elements are interpreted as related but independent.2
Proximity is one of the most powerful means of indicating relatedness in a design,
and will generally overwhelm competing visual cues (e.g., similarity). Arrange
elements such that their proximity corresponds to their relatedness. Ensure that
labels and supporting information are near the elements that they describe,
opting for direct labeling on graphs over legends or keys. Locate unrelated or
ambiguously related items relatively far from one another.
See also Chunking, Performance Load, and Similarity.

1 The seminal work on proximity is “Untersuch-
ungen zür Lehre von der Gestalt, II” [Laws
of Organization in Perceptual Forms] by Max
Wertheimer, Psychologische Forschung, 1923,
vol. 4, p. 301–350, reprinted in A Source Book
of Gestalt Psychology by Willis D. Ellis (ed.),
Routledge & Kegan Paul, 1999, p. 71–88. See
also Principles of Gestalt Psychology by Kurt
Koffka, Harcourt Brace, 1935.
2 Euler circles and Venn diagrams (methods
of illustrating the relationships between sets
of things in logic and mathematics) utilize
this principle.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

C	A 	B
E
F	D
Proximity between the circles
influences how they are grouped—as
columns, a square group of circles,
or rows.
Circles A and B are perceived as
independent and sharing no attributes.
Circles C and D are perceived as
partially dependent and sharing some
attributes. Circle F is perceived as
dependent on Circle E and sharing all
of its attributes.
This rendering of a sign at Big Bend
National Park has undoubtedly
sent many hikers in unintended
directions (two hikers for certain). The
proximity between unrelated words
(e.g., Chisos and South) lends itself
to misinterpretation. Positioning the
related words closer together corrects
the problem.
Window controls are often placed on
the center console between seats. The
lack of proximity between the controls
and the window makes it a poor
design. A better location would be on
the door itself.
Proximity 197

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Proximity** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Proximity để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Performance Load, and Similarity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
