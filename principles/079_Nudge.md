---
name: "Nudge"
vi: "Cú hích hành vi (Nudge)"
summary: "Nudge (Cú hích hành vi (Nudge)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Nudge (Cú hích hành vi (Nudge))

> **Tóm tắt cốt lõi (Summary)**: Nudge là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Nudge
A method for predictably altering behavior without
restricting options or significantly changing incentives.1
People prefer the path of least resistance when making decisions. When the path
of least resistance happens to lead to a generally favorable outcome everyone is
happy. When the path of least resistance leads to a generally unfavorable
outcome, however, the results are problematic. For example, when the default
option for new employees is to not be registered for a basic pension program,
savings rates are very low. However, when the default option is to enroll
employees automatically into a basic pension plan, savings rates increase
dramatically. In both cases, employees are free to join, change plans, or not join,
but intelligent defaults nudge employees to make the most responsible decision
The following methods are common nudging techniques:
Defaults — Select defaults that do the least harm and most good (e.g., many
lives are lost due to lack of available organ donations, a shortage that could be
addressed by changing the default enrollment from opt-in to opt-out).
Feedback — Provide visible and immediate feedback for actions and inactions
(e.g., many modern automobiles have alert lights on the dashboard that stay on
until the seatbelt is fastened, increasing seatbelt usage).
Incentives — Avoid incentive conflicts and align incentives to preferred
behaviors (e.g., the “Cash for Clunkers” legislation passed in the United States
in 2009 provided a cash incentive for consumers to trade in older cars for new
cars, boosting sales for the ailing automotive industry and reducing total energy
consumption and pollution).
Structured Choices — Provide the means to simplify and filter complexity to
facilitate decision making (e.g., Netflix structures choices for customers to help
them find movies, enabling them to search and browse based on titles, actors,
directors, genres, and the recommendations of other customers).
Visible Goals — Make simple performance measures clearly visible so that
people can immediately assess their performance against a goal state (e.g.,
clearly displaying manufacturing output and goals in factories is often, by itself,
sufficient to increase productivity).2
Consider nudges in the design of objects and environments where behavior
modification is key. Set default states that correspond to the most generally
desired option, not the most conservative option. Provide clear, visible, and
immediate feedback to reinforce desired actions and mildly punish undesired
behaviors. Align incentives with desired behaviors, being careful to avoid incentive
conflict. Simplify and structure choices when decision-making parameters are
complex. Make goals and performance status clearly visible.
See also Affordance, Confirmation, Constraint, Framing, and Mapping.
1 Also known as choice architecture.
2 The seminal work on nudges is Nudge:
Improving Decisions About Health, Wealth,
and Happiness by Richard Thaler and Cass
Sunstein, Penguin, 2008. See also Choices,
Values, and Frames by Daniel Kahneman
and Amos Tversky, Cambridge University
Press, 2000.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Nudge 171
To reduce the cleaning burden
of the men’s restrooms in the
Schiphol airport in Amsterdam, the
image of a fly was etched into each of
the bowls just above the drains. The
result was an 80 percent reduction in
“spillage.” Why? When people see a
target, they try to hit it.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Nudge** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Nudge để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Confirmation, Constraint, Framing, and Mapping
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
