---
name: "Performance Load"
vi: "Tải trọng hiệu năng (Cognitive & Kinematic Load)"
summary: "Performance Load (Tải trọng hiệu năng (Cognitive & Kinematic Load)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - usability
---

# Universal Design Principle: Performance Load (Tải trọng hiệu năng (Cognitive & Kinematic Load))

> **Tóm tắt cốt lõi (Summary)**: Performance Load là một nguyên lý thiết kế then chốt thuộc nhóm **learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Performance Load
The greater the effort to accomplish a task, the less likely
the task will be accomplished successfully.1
Performance load is the degree of mental and physical activity required to
achieve a goal. If the performance load is high, performance time and errors
increase, and the probability of successfully accomplishing the goal decreases.
If the performance load is low, performance time and errors decrease, and the
probability of successfully accomplishing the goal increases. Performance load
consists of two types of loads: cognitive load and kinematic load.2
Cognitive load is the amount of mental activity—perception, memory, problem
solving—required to accomplish a goal. For example, early computer systems
required users to remember large sets of commands, and then type them into the
computer in specific ways. The number of commands that had to be remembered
to perform a task was the cognitive load for that task. The advent of the graphical
user interface allowed users to browse sets of commands in menus, rather than
recalling them from memory. This reduction in cognitive load dramatically reduced
the mental effort required to use computers, and consequently enabled them
to become mass-market devices. General strategies for reducing cognitive load
include minimizing visual noise, chunking information that must be remembered,
using memory aids to assist in recall and problem solving, and automating
computation- and memory-intensive tasks.
Kinematic load is the degree of physical activity—number of steps or movements,
or amount of force—required to accomplish a goal. For example, the telegraph
required people to communicate letters one at a time through a series of taps
on a mechanical armature. The number of taps to communicate a message was
the kinematic load for that task. Samuel Morse designed Morse code to minimize
kinematic load by assigning the simplest codes to the most frequently occurring
letters; the letter E was expressed as dot, and the letter Q was expressed as the
longer dash dash dot dash. This approach reduced the physical effort (kinematic
load), dramatically reducing transmission times and error rates. General strategies
for reducing kinematic load include reducing the number of steps required to
complete tasks, minimizing range of motion and travel distances, and automating
repetitive tasks.3
Design should minimize performance load to the greatest degree possible. Reduce
cognitive load by eliminating unnecessary information from displays, chunking
information that is to be remembered, providing memory aids to assist in complex
tasks, and automating computation-intensive and memory-intensive tasks. Reduce
kinematic load by reducing unnecessary steps in tasks, reducing overall motion
and energy expended, and automating repetitive tasks.
See also 80/20 Rule, Chunking, Cost-Benefit, Hick’s Law, Fitts’ Law, Mnemonic
Device, and Recognition Over Recall.

1 Also known as the path-of-least-resistance
principle and principle of least effort.
2 The seminal works on performance load
are Cognitive Load During Problem Solving:
Effects on Learning by John Sweller, Cognitive
Science, 1988, vol. 12, p. 257–285; “The
Magical Number Seven, Plus or Minus
Two: Some Limits on Our Capacity for
Processing Information” by George Miller, The
Psychological Review, 1956, vol. 63, p. 81–97;
and Human Behavior and The Principle
of Least Effort by George K. Zipf, Addison-
Wesley, 1949.
3 “Frustrations of a Pushbutton World” by
Harold Thimbleby, Encyclopedia Britannica
Yearbook of Science and the Future, 1992, p.
202–219.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Insert your
casino player's
card and push
the button.
$UPER
JACKPOT
$UPER	$UPER
JACKPOT	JACKPOT
Modern slot machines no longer
require the pulling of a lever or the
insertion of coins to play. Inserting a
charge card and pressing a button is
all that is required, though the lever
continues to be retained as a usable
ornament. This reduction in kinematic
load not only makes it easier to play
the slots, it makes it easier for casinos
to make money.
Remote keyless entry enables people
to lock and unlock all doors of a
vehicle at the press of a button—a
dramatic reduction in kinematic load.
People can easily save their favorite
Internet destinations in all modern
browsers. This feature replaces the
more load-intensive alternatives of
remembering destinations, or writing
them down.
The use of Universal Product
Codes, also known as bar codes,
dramatically reduces the performance
load associated with consumer
transactions: products no longer need
price tags, cashiers no longer need
to type in prices, and inventory is
automatically updated.
Performance Load 179
Bookmarks
Add Page
Organize
magazines
info design
references
cool sites
tech reference
shopping
furniture
recipes
Multimedia
Hardware Developers
Software Developers
Toolbar Favorites
Project Management Glossary
Web Redesign
Tutorials > Javascript
Fonts Order Form

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Performance Load** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Performance Load để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Chunking, Cost-Benefit, Hick’s Law, Fitts’ Law, Mnemonic
Device, and Recognition Over Recall
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
