---
name: "Constraint"
vi: "Ràng buộc thao tác (Constraint)"
summary: "Constraint (Ràng buộc thao tác (Constraint)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Constraint (Ràng buộc thao tác (Constraint))

> **Tóm tắt cốt lõi (Summary)**: Constraint là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A method of limiting the actions that can be performed on
a system.
Constraints limit the possible actions that can be performed on a system. For
example, dimming or hiding unavailable software controls constrains the options
that can be selected. Proper application of constraints in this fashion makes
designs easier to use and dramatically reduces the probability of error during
interaction. There are two basic kinds of constraints: physical constraints and
psychological constraints.1
Physical constraints limit the range of possible actions by redirecting physical
motion in specific ways. The three kinds of physical constraints are paths, axes,
and barriers. Paths convert applied forces into linear or curvilinear motion using
channels or grooves (e.g., scroll bar in software user interfaces). Axes convert
applied forces into rotary motion, effectively providing a control surface of infinite
length in a small space (e.g., a trackball). Barriers absorb or deflect applied
forces, thereby halting, slowing, or redirecting the forces around the barrier (e.g.,
boundaries of a computer screen). Physical constraints are useful for reducing the
sensitivity of controls to unwanted inputs, and denying certain kinds of inputs
altogether. Paths are useful in situations where the control variable range is
relatively small and bounded. Axes are useful in situations where control real
estate is limited, or the control variables are very large or unbounded. Barriers are
useful for denying errant or undesired actions.
Psychological constraints limit the range of possible actions by leveraging the
way people perceive and think about the world. The three kinds of psychological
constraints are symbols, conventions, and mappings. Symbols influence behavior
by communicating meaning through language, such as the text and icon on a
warning sign. Conventions influence behavior based on learned traditions and
practices, such as “red means stop, green means go.” Mappings influence
behavior based on the perceived relationships between elements. For example,
light switches that are close to a set of lights are perceived to be more related
than switches that are far away. Symbols are useful for labeling, explaining, and
warning using visual, aural, and tactile representation—all three if the message is
critical. Conventions indicate common methods of understanding and interacting,
and are useful for making systems consistent and easy to use. Mappings are
useful for implying what actions are possible based on the visibility, location, and
appearance of controls.2
Use constraints in design to simplify usability and minimize errors. Use physical
constraints to reduce the sensitivity of controls, minimize unintentional inputs,
and prevent or slow dangerous actions. Use psychological constraints to improve
the clarity and intuitiveness of a design.
See also Affordance, Archetypes, Control, Errors, Forgiveness, Mapping, and Nudge.

1 The seminal work on psychological constraints
is The Design of Everyday Things by Donald
Norman, Doubleday, 1990.
2 Note that Norman uses the terms semantic
constraints, cultural constraints, and logical
constraints.
Constraint

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Physical Constraints
Paths
Axes
Barriers
Constraint 61
ROAD
MAX
A/C
A/C
VENT OFF
CROSSING
RAIL
RECORD	STOP/EJECT
FF	PLAY	REW
Psychological Constraints
Symbols
POISON 	WOMEN
Conventions
Mappings
Volume 	Back 	Next
Brightness
Contrast
Hue
Saturation

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Constraint** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Constraint để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Archetypes, Control, Errors, Forgiveness, Mapping, and Nudge
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
