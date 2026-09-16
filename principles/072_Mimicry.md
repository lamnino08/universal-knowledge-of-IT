---
name: "Mimicry"
vi: "Phỏng sinh học và mô phỏng (Mimicry)"
summary: "Mimicry (Phỏng sinh học và mô phỏng (Mimicry)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
  - usability
---

# Universal Design Principle: Mimicry (Phỏng sinh học và mô phỏng (Mimicry))

> **Tóm tắt cốt lõi (Summary)**: Mimicry là một nguyên lý thiết kế then chốt thuộc nhóm **appeal, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Mimicry
The act of copying properties of familiar objects,
organisms, or environments in order to realize specific
benefits afforded by those properties.
In nature, mimicry refers to the copying of properties of familiar objects,
organisms, or environments in order to hide from or deter other organisms. For
example, katydids and walking sticks mimic the leaves and branches of plants
to hide from predators, and the viceroy butterfly mimics the less tasty monarch
butterfly to deter predators. In design, mimicry refers to copying properties of
familiar objects, organisms, or environments in order to improve the usability,
likeability, or functionality of an object. There are three basic kinds of mimicry in
design: surface, behavioral, and functional.1
Surface mimicry is defined as making a design look like something else. When a
design mimics the surface aspects of a familiar object, the design implies (by its
familiar appearance) the way it will function or can be used. An example is the use
of computer software icons that are designed to look like folders and documents.2
Behavioral mimicry is defined as making a design act like something else
(e.g., making a robotic dog act like a real dog). Behavioral mimicry is useful for
improving likeability, but should be used with caution when mimicking complex
behaviors from large repertoires. For example, mimicking behaviors like smiling
generally elicit positive responses, but can give the impression of artificiality
or deceit if inconsistent with other cues (e.g., a baby doll that smiles when
touched—or spanked).3
Functional mimicry is defined as making a design work like something else.
Functional mimicry is useful for solving mechanical and structural problems
(e.g., mimicking the keypad of an adding machine in the design of a touch tone
telephone). Significant insights and rapid progress can be achieved by mimicking
existing solutions and design analogs. However, functional mimicry must be
performed with caution since the physical principles governing function may
not transfer from one context to another or from one scale to another (e.g., early
attempts at human flight by flapping wings).4
Mimicry is perhaps the oldest and most efficient method for achieving major
advances in design. Consider surface mimicry to improve usability, ensuring that
the perception of the design corresponds to how it functions or is to be used.
Consider behavioral mimicry to improve likeability, but exercise caution when
mimicking complex behaviors. Consider functional mimicry to assist in solving
mechanical and structural problems, but also consider transfer and scaling effects
that may undermine the success of the mimicked properties.
See also Affordance, Anthromorphic Form, Baby-Face Bias, Convergence,
Savanna Preference, and Scaling Fallacy.

1 The history of mimicry in design likely pre-
dates the development of tools by early
humans. The seminal work on mimicry in
plants and animals was performed by Henry
Bates and Fritz Muller in the late 1800s.
2 See, for example, The Design of Everyday
Things by Donald Norman, Doubleday, 1990.
3 See, for example, Designing Sociable Robots
by Cynthia L. Breazeal, MIT Press, 2002; and
“The Lovable Cat: Mimicry Strikes Again” in
The Throwing Madonna: Essays on the Brain
by William H. Calvin, iUniverse, 2000.
4 See, for example, Biomimicry: Innovation
Inspired by Nature by Janine M. Benyus,
William Morrow & Company, 1998; and Cats’
Paws and Catapults: Mechanical Worlds of
Nature and People by Steven Vogel, W. W.
Norton & Company, 2000.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Mimicry 157
Trash 	Recycle Bin 	Documents 	Work 	Document 	Data.txt
The Mimic Octopus is capable of both
surface and behavioral mimicry, in this
case changing its pattern and texture,
and hiding all but two legs in order to
mimic the highly poisonous Sea Snake.
The Sony AIBO mimics many key
canine behaviors—barking, wagging
tail—leveraging the positive feelings
many people have for dogs to make
the design more appealing.
Mimicry is an effective strategy to
begin exploring a design problem,
but it should not be assumed that
mimicked solutions are correct or
best. For example, the early design
of the phone keypad mimicked
the keypad of adding machines.
Usability testing by researchers at
Bell Laboratories suggested that an
inverted keypad layout was easier to
master. Bell decided to abandon the
mimicked solution and establish a new
standard for telephones.
Surface mimicry is common in the
design of software icons and controls.
Even to those unfamiliar with the
software, the familiar appearance of
these objects hints at their function.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Mimicry** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Mimicry để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Anthromorphic Form, Baby-Face Bias, Convergence,
Savanna Preference, and Scaling Fallacy
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
