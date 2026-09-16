---
name: "Operant Conditioning"
vi: "Phản xạ có điều kiện tạo tác"
summary: "Operant Conditioning (Phản xạ có điều kiện tạo tác): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - appeal
---

# Universal Design Principle: Operant Conditioning (Phản xạ có điều kiện tạo tác)

> **Tóm tắt cốt lõi (Summary)**: Operant Conditioning là một nguyên lý thiết kế then chốt thuộc nhóm **learning, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Operant Conditioning
A technique used to modify behavior by reinforcing
desired behaviors, and ignoring or punishing
undesired behaviors.1
Operant conditioning is probably the most researched and well-known technique
used to modify behavior. The technique involves increasing or decreasing a
particular behavior by associating the behavior with a positive or negative condition
(e.g., rewards or punishments). Operant conditioning is commonly applied to
animal training, instructional design, video game design, incentive programs,
gambling devices, counseling, and behavioral therapy. It is also finding increased
application in artificial intelligence. There are three basic operant conditioning
techniques: positive reinforcement, negative reinforcement, and punishment.2
Positive reinforcement increases the probability of a behavior by associating the
behavior with a positive condition; pulling the lever on a slot machine results in
positive visual and auditory feedback, and a possible monetary reward. Negative
reinforcement increases the probability of a behavior by associating the behavior
with the removal of a negative condition; fastening a seat belt in a car silences
an annoying buzzer. Punishment decreases the probability of a behavior by
associating the behavior with a negative condition; touching a poison mushroom
in a video game reduces the score. Positive and negative reinforcement should be
used instead of punishment whenever possible. Punishment should be reserved
for rapidly extinguishing a behavior, or it should not be used at all.
Reinforcement and punishment are administered after a behavior is performed
one or more times. When there is a clear and predictive relationship between the
frequency of a behavior and an outcome, behavior will be paced to do just what is
required to receive reinforcement or avoid punishment. When there is not a clear
and predictive relationship between the frequency of behavior and the outcome,
behavior will be performed more frequently and will be more resistant to extinction
(the loss of the desired behavior). An optimal behavior modification plan typically
includes predictable reinforcement early in training (fixed ratio schedules) and less
predictable reinforcement later in the training (variable ratio schedules).
Use operant conditioning in design contexts where behavioral change is required.
Focus on positive or negative reinforcement, rather than punishment whenever
possible. Use fixed ratio schedules of reinforcement early in training. As basic
behaviors are mastered, switch to variable schedules of reinforcement.
See also Classical Conditioning and Shaping.

1 Also known as instrumental conditioning.
2 The seminal work on operant conditioning is
The Behavior of Organisms: An Experimental
Analysis by Burrhus F. Skinner, Appleton-
Century, 1938; a nice contemporary book on
the subject is Don’t Shoot the Dog: The New
Art of Teaching and Training by Karen Pryor,
Bantam Doubleday Dell, 1999.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

This graph shows how reinforcement
strategies influence the frequency
of behavior. Variable ratio schedules
provide reinforcement after a variable
number of correct responses. They
ultimately achieve the highest fre-
quency of behavior and are useful
for maintaining behavior. Fixed ratio
schedules provide reinforcement after
a fixed number of correct responses.
They are useful for connecting the
reinforcement to the behavior during
the early stages of learning.
The addictive nature of video
games and gambling machines is
a direct result of their application of
operant conditioning.
In the game Black & White, the
nature of the characters evolve to
become good, neutral, or evil based
on how their behaviors are rewarded
and punished.
1UP
SCORE 60 	HIGH SCORE 105450
Operant Conditioning 175
Variable Ratio
Time
Cumulative Behavior
Fixed Ratio

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Operant Conditioning** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Operant Conditioning để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Classical Conditioning and Shaping
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
