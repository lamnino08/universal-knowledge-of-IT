---
name: "Shaping"
vi: "Định hình hành vi từng bước (Shaping)"
summary: "Shaping (Định hình hành vi từng bước (Shaping)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
---

# Universal Design Principle: Shaping (Định hình hành vi từng bước (Shaping))

> **Tóm tắt cốt lõi (Summary)**: Shaping là một nguyên lý thiết kế then chốt thuộc nhóm **learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Shaping
A technique used to teach a desired behavior by reinforcing
increasingly accurate approximations of the behavior.1
Complex behaviors can be difficult to teach. Shaping is a strategy whereby
complex behaviors are broken down into smaller, simpler subbehaviors, and then
taught one by one. The behaviors are reinforced (e.g., given food), and ultimately
chained together to achieve a desired result. For example, to teach a mouse
to press a lever, the mouse is first reinforced to move close to the lever; then
reinforced only when it makes contact with the lever; and eventually only when it
presses the lever.2
Often, shaping occurs without awareness. For example, video games use shaping
when initial game levels require simple inputs in order to “beat” the level (obtain
the reinforcement), and then require increasingly difficult controller actions to
master higher levels of the game. Salespeople use a form of shaping when they
offer a prize to come to their location, provide food and drink to discuss the sale,
and then offer a discount for making a purchase decision that day. Each action
toward the goal behavior (making the sale) is reinforced.
During shaping, behaviors that have nothing to do with the desired behavior
can get incidentally reinforced. For example, when training a mouse to press
a lever, the mouse may incidentally press a lever with one foot in the air. The
reinforcement for the lever press may also inadvertently reinforce the fact that the
foot was in the air. This behavior then becomes an integrated, but unnecessary
component of the desired behavior; the mouse lifts its foot whenever it presses
the lever. The development of this kind of superstitious behavior is common with
humans as well.
Use shaping to train complex behaviors in games, simulations, and learning
environments. Shaping does not address the “hows” or “whys” of a task, and
should, therefore, primarily be used to teach rote procedures and refine complex
motor tasks. Shaping is being increasingly used to train complex behaviors in
artificial beings, and should be considered when developing adaptive systems.3
See also Classical Conditioning and Operant Conditioning.

1 Also known as approximation conditioning and
conditioning by successive approximations.
2 The seminal work on shaping is The Behavior
of Organisms: an Experimental Analysis by
B. F. Skinner, Appleton-Century, 1938. An
excellent account of Skinner’s early research
and development is “Engineering Behavior:
Project Pigeon, World War II, and the
Conditioning of B. F. Skinner” by James H.
Capshew, Technology and Culture, 1993,
vol. 34, p. 835–857.
3 See, for example, Robot Shaping: An
Experiment in Behavior Engineering by Marco
Dorigo and Marco Colombetti, MIT Press, 1997.
Moving 	Touching 	Pressing

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Project Pigeon
Project Pigeon was a classified
research-and-development program
during World War II. It was developed
at a time when electronic guidance
systems did not exist, and the only
compensation for the inaccuracy of
bombs was dropping them in quantity.
This ingenious application of shaping
would have dramatically increased the
accuracy of bombs and decreased
civilian casualties. Despite favorable
performance tests, however, the
National Defense Research Committee
ended the project—it seems they
couldn’t get over the idea that pigeons
would be guiding their bombs.
Shaping 223
1. Pigeons were trained to peck at
targets on aerial photographs. Once
a certain level of proficiency was
obtained, pigeons were jacketed
and mounted inside tubes.
2. The pigeons in their tubes were
inserted into the nosecone of
the bomb. Each nosecone used
three pigeons in a type of voting
system, whereby the pigeon
pecks of two birds in agreement
would overrule the errant pigeon
pecks of a single bird.
3. Sealed in the bomb, the pigeons
could see through glass lenses in
the nosecone.
4. Once the bomb was released,
the pigeons would begin pecking
at their view of the target. Their
pecks shifted the glass lens off-
center, which adjusted the bomb’s
tail surfaces and, correspondingly,
its trajectory.
1
2
3
4

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Shaping** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Shaping để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Classical Conditioning and Operant Conditioning
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
