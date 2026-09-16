---
name: "Control"
vi: "Kiểm soát người dùng (Control)"
summary: "Control (Kiểm soát người dùng (Control)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Control (Kiểm soát người dùng (Control))

> **Tóm tắt cốt lõi (Summary)**: Control là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The level of control provided by a system should be
related to the proficiency and experience levels of the
people using the system.
People should be able to exercise control over what a system does, but the level
of control should be related to their proficiency and experience using the system.
Beginners do best with a reduced amount of control, while experts do best with
greater control. A simple example is when children learn to ride a bicycle. Initially,
training wheels are helpful in reducing the difficulty of riding by reducing the
level of control (e.g., eliminating the need to balance while riding). This allows the
child to safely develop basic riding skills with minimal risk of accident or injury.
Once the basic skills are mastered, the training wheels get in the way, and hinder
performance. As expertise increases, so too does the need for greater control.1
A system can accommodate these varying needs by offering multiple ways to
perform a task. For example, novice users of word processors typically save
their documents by accessing the File menu and selecting Save, whereas more
proficient users typically save their documents using a keyboard shortcut. Both
methods achieve the same outcome, but one favors simplicity and structure,
while the other favors efficiency and flexibility. This tradeoff is standard when
allocating system control. Beginners benefit from structured interactions with
minimal choices, typically supported by prompts, constraints, and ready access
to help. Experts benefit from less structured interactions that provide more
direct access to functions, bypassing the support devices of beginners. Since
accommodating multiple methods increases the complexity of the system,
the number of methods for any given task should be limited to two—one for
beginners, and one for experts.
The need to provide expert shortcuts is limited to systems that are used frequently
enough for people to develop expertise. For example, the design of museum
kiosks and ATMs should assume that all users are first-time users, and not try
to accommodate varying levels of expertise. When systems are used frequently
enough for people to develop expertise, it is often useful to provide simple ways
to customize the system design. This represents the highest level of control a
design can provide. It enables the appearance and configuration of a system
to be aligned with personal preferences and level of expertise, and enables the
efficiency of use to be fine-tuned according to individual needs over time.
Consider the allocation of control in the design of complex systems. When
possible, use a method that is equally simple and efficient for beginners and
experts. Otherwise, provide methods specialized for beginners and experts.
Conceal expert methods to the extent possible to minimize complexity for
beginners. When systems are complex and frequently used, consider designs that
can be customized to conform to individual preference and levels of expertise.
See also Constraint, Flexibility-Usability Tradeoff, and Hierarchy of Needs.

1 See, for example, The Psychology of Human-
Computer Interaction by Stuart K. Card,
Thomas P. Moran, and Allen Newell, Lawrence
Erlbaum Associates, 1983; and The Humane
Interface: New Directions for Designing
Interactive Systems by Jef Raskin, Addison-
Wesley 2000.
Control

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

One method of accommodating
variations in proficiency is to provide
different methods of interaction for
beginners and experts. For example,
Macromedia Flash supports novice
and expert developers by providing
different user modes when writing
scripts. Selecting the Expert Mode
permits unconstrained command
entry into the editor field. Selecting
Normal Mode permits constrained
entry only, requiring commands to be
entered into specialized fields so that
they can be immediately checked
for correctness.
Control 65
Actions - Frame
Actions for Frame 1 of Layer Name Layer 1
gotoAndStop(1);
Line 2 of 2, Col 1
Normal Mode
Expert Mode
View Line Numbers
Actions - Frame
Actions for Frame 1 of Layer Name Layer 1
goto: Go to the specified frame of the movie
Go to and Play 	Go to and Stop
Scene: <current scene>
Type: Frame Number
Frame:
gotoAndStop(1);
Line 1: gotoAndStop(1);
Normal Mode
Expert Mode
View Line Numbers

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Control** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Control để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Constraint, Flexibility-Usability Tradeoff, and Hierarchy of Needs
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
