---
name: "Layering"
vi: "Phân tầng thông tin (Layering)"
summary: "Layering (Phân tầng thông tin (Layering)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - learning
  - usability
---

# Universal Design Principle: Layering (Phân tầng thông tin (Layering))

> **Tóm tắt cốt lõi (Summary)**: Layering là một nguyên lý thiết kế then chốt thuộc nhóm **perception, learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Layering
The process of organizing information into related
groupings in order to manage complexity and reinforce
relationships in the information.
Layering involves organizing information into related groupings and then
presenting or making available only certain groupings at any one time. Layering
is primarily used to manage complexity, but can also be used to reinforce
relationships in information. There are two basic kinds of layering: two-dimensional
and three-dimensional.1
Two-dimensional layering involves separating information into layers such that
only one layer of information can be viewed at a time. Two-dimensional layers can
be revealed in either a linear or nonlinear fashion. Linear layers are useful when
information has a clear beginning, middle, and end (e.g., stories), and are revealed
successively like pages in a book. Nonlinear layers are useful when reinforcing
relationships between the layers. The types of nonlinear layer relationships can
be hierarchical, parallel, or web. Hierarchical layers are useful when information
has superordinate and subordinate relationships within itself (e.g., organizational
chart), and are revealed top-down or bottom-up in rigid accordance with the
hierarchical structure. Parallel layers are useful when information is based on the
organization of other information (e.g., thesaurus), and are revealed through some
correspondence with that organization. Web layers are useful when information
has many different kinds of relationships within itself (e.g., hypertext), and are
revealed through any number of associative linkages to other layers.
Three-dimensional layering involves separating information into layers such
that multiple layers of information can be viewed at a time. Three-dimensional
layers are revealed as either opaque or transparent planes of information that
sit atop one another (i.e., in a third dimension). Opaque layers are useful when
additional information about a particular item is desired without switching
contexts (e.g., software pop-up windows). Transparent layers are useful when
overlays of information combine to illustrate concepts or highlight relationships
(e.g., weather maps). 2
Use two-dimensional layering to manage complexity and direct navigation through
information. Consider linear layers when telling stories and presenting sequences
of time-based events, and use nonlinear layers when emphasizing relationships
within the information. Use three-dimensional layering to elaborate information
and illustrate concepts without switching contexts. Consider opaque layers when
presenting elaborative information, and transparent layers when illustrating
concepts or highlighting relationships in information.
See also Chunking, Five Hat Racks, Progressive Disclosure, and Propositional
Density.

1 A similar concept is found in Designing
Business: Multiple Media, Multiple Disciplines
by Clement Mok, Adobe Press, 1996, p.
102–107 [Organizational Models].
2 See, for example, Envisioning Information by
Edward R. Tufte, Graphics Press, 1998, p.
53–65; 81–95 [Layering and Separation; Color
and Information].

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

90º
62º
87º 71º
65º
Olympia
Salem
Sacramento
Phoenix
Olympia
Salem
Sacramento
Phoenix is the
capital of Arizona
Layering 147
Two-dimensional layering is useful for
presentation and navigation. Layers
are revealed one at a time, like pages
in a book.
Three-dimensional layering is useful
for elaboration and highlighting.
Relationships and patterns on
one layer of information (left) are
elaborated by layers of information
that pop up or overlay (right).
Two-Dimensional Layering 	Three-Dimensional Layering
Linear 	Opaque
Beginning 	Middle 1 	Middle 2 	End
Nonlinear
Hierarchical President
Vice 	Vice
President 	President
Services 	Products
Sales 	Production	Manager Manager 	Manager
Parallel Word 	Synonym
Word 	Synonym
Word 	Synonym
Web 	Related
Information
Related 	Related 	Home 	Related
Information 	Information 	Page 	Information
Related 	Related
Information 	Information
Transparent

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Layering** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Layering để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Five Hat Racks, Progressive Disclosure, and Propositional
Density
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
