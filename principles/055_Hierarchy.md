---
name: "Hierarchy"
vi: "Hệ thống phân cấp (Hierarchy)"
summary: "Hierarchy (Hệ thống phân cấp (Hierarchy)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - usability
---

# Universal Design Principle: Hierarchy (Hệ thống phân cấp (Hierarchy))

> **Tóm tắt cốt lõi (Summary)**: Hierarchy là một nguyên lý thiết kế then chốt thuộc nhóm **learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Hierarchy
Hierarchical organization is the simplest structure for
visualizing and understanding complexity.
Increasing the visibility of the hierarchical relationships within a system is one of
the most effective ways to increase knowledge about the system. Examples of
visible hierarchies are book outlines, multi-level software menus, and classification
diagrams. Perception of hierarchical relationships among elements is primarily a
function of their relative left-right and top-down positions, but is also influenced
by their proximity, size, and the presence of connecting lines. Superordinate
elements are commonly referred to as parent elements, and subordinate elements
as child elements. There are three basic ways to visually represent hierarchy:
trees, nests, and stairs.1
Tree structures illustrate hierarchical relationships by locating child elements
below or to the right of parent elements, or through the use of other strategies
indicating hierarchy (e.g., size, connecting lines). Tree structures are effective for
representing hierarchies of moderate complexity, but can become cumbersome
for large or complex hierarchies. Tree structures grow large quickly, and become
tangled when multiple parents share common child elements. Tree structures are
commonly used to represent overviews or high-level maps of system organization.
Nest structures illustrate hierarchical relationships by visually containing child
elements within parent elements, as in a Venn diagram. Nest structures are most
effective when representing simple hierarchies. When the relationships between
the different levels of the hierarchy become too dense and complex to be clearly
distinguishable, nest structures become less effective. Nest structures are most
commonly used to group information and functions, and to represent simple
logical relationships.
Stair structures illustrate hierarchical relationships by stacking child elements
below and to the right of parent elements, as in an outline. Stair structures are
effective for representing complex hierarchies, but are not easily browsed, and
falsely imply a sequential relationship between the stacked child elements.
Interactive stair structures found in software often deal with the former problem by
concealing child elements until a parent element is selected. Stair structures are
commonly used to represent large system structures that change over time.2
Hierarchical representation is the simplest method of increasing knowledge about
the structure of a system. Consider tree structures when representing high-level
views of hierarchies of moderate complexity. Consider nest structures when
representing natural systems, simple hierarchical relationships, and grouped
information or functions. Consider stair structures when representing complex
hierarchies, especially if the volatility and growth of the system represented is
unpredictable. Explore ways to selectively reveal and conceal the complexity of
hierarchical structures to maximize their clarity and effectiveness.3
See also Advance Organizer, Alignment, Five Hat Racks, Layering, and Proximity.
1 The seminal works on hierarchy are “The
Architecture of Complexity,” Proceedings of
the American Philosophical Society, 1962,
vol. 106, p. 467–482; and The Sciences of
the Artificial, MIT Press, 1969, both by Herbert
A. Simon.
2 Note that stair hierarchies in software are often
referred to as tree hierarchies.
3 Representing these structures in three-
dimensional space improves little in terms of
clarity and comprehensibility—though it does
result in some fascinating structures to view
and navigate. See, for example, “Cone Trees:
Animated 3D Visualizations of Hierarchical
Information” by George G. Robertson, Jock D.
Mackinlay, Stuart K. Card, Proceedings of CHI
’91: Human Factors in Computing Systems,
1991, p. 189–194.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Hierarchy 123
Nests
Stairs
Trees
purposeful
arrangement drawing or
sketch	conceive or
fashion
invent
devise
intent
purpose
blueprint
graphic
representation
aim
intention
pattern
project
design
create in an
artistic manner
form
a plan
figure

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Hierarchy** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Hierarchy để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Advance Organizer, Alignment, Five Hat Racks, Layering, and Proximity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
