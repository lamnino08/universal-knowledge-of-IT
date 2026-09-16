---
name: "Rule of Thirds"
vi: "Quy tắc một phần ba (Rule of Thirds)"
summary: "Rule of Thirds (Quy tắc một phần ba (Rule of Thirds)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Rule of Thirds (Quy tắc một phần ba (Rule of Thirds))

> **Tóm tắt cốt lõi (Summary)**: Rule of Thirds là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

1 Also known as golden grid rule.
2 A nice introduction to compositional concepts
is Design and Composition by Nathan
Goldstein, Prentice-Hall, 1997.

Rule of Thirds
A technique of composition in which a medium is divided
into thirds, creating aesthetic positions for the primary
elements of a design. 1
The rule of thirds is a technique derived from the use of early grid systems in
composition. It is applied by dividing a medium into thirds both vertically and
horizontally, creating an invisible grid of nine rectangles and four intersections.
The primary element within a design is then positioned on an intersection of the
grid. The asymmetry of the resulting composition is interesting to look at, and
generally agreed to be aesthetic.
The technique has a loyal following in design circles due to its use by the
Renaissance masters and its rough relationship to the golden ratio. Although
dividing a design into thirds yields a ratio different from the golden ratio (i.e.,
the 2/3 section = 0.666 versus golden ratio = 0.618), the users of the technique
may have decided that the simplicity of its application compensated for its
rough approximation.
The rule of thirds generally works well, is easy to apply, and should be considered
when composing elements of a design. When the primary element is so strong
as to imbalance the composition, consider centering the element rather than
using the rule of thirds—especially when the strength of the primary element is
reinforced by the surrounding elements or space. If the surrounding elements
or space do not reinforce the primary element, use the rule of thirds and add a
secondary element (known as a counterpoint) to the opposing intersection of the
primary element to bring the composition to balance. In designs where there is a
strong vertical or horizontal element, it is common practice to align the element
along one of the grid lines of corresponding orientation.2
See also Alignment, Golden Ratio, and Symmetry.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Rule of Thirds 209
This photograph (above) from the
Muhammad Ali–Joe Frazier fight in
Manila, Philippines (1975) makes
excellent use of the rule of thirds,
placing the heads of both fighters at
opposing intersections on the grid.
This photograph (right) from the
Muhammad Ali–Sonny Liston fight in
Lewiston, Maine (1965), by contrast,
is an excellent example of when not
to use the rule of thirds—strong
primary element that is reinforced by
the surrounding space.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Rule of Thirds** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Rule of Thirds để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Alignment, Golden Ratio, and Symmetry
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
