---
name: "Feedback Loop"
vi: "Vòng phản hồi (Feedback Loop)"
summary: "Feedback Loop (Vòng phản hồi (Feedback Loop)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Feedback Loop (Vòng phản hồi (Feedback Loop))

> **Tóm tắt cốt lõi (Summary)**: Feedback Loop là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A relationship between variables in a system where the
consequences of an event feed back into the system as
input, modifying the event in the future.
Every action creates an equal and opposite reaction. When reactions loop back to
affect themselves, a feedback loop is created. All real-world systems are compose
of many such interacting feedback loops—animals, machines, businesses, and
ecosystems, to name a few. There are two types of feedback loops: positive
and negative. Positive feedback amplifies system output, resulting in growth or
decline. Negative feedback dampens output, stabilizing the system around an
equilibrium point.1
Positive feedback loops are effective for creating change, but generally result
in negative consequences if not moderated by negative feedback loops. For
example, in response to head and neck injuries in football in the 1950s, designers
created plastic football helmets with internal padding to replace leather helmets.
The helmets provided more protection, but induced players to take increasingly
greater risks when tackling. More head and neck injuries occurred than before.
By concentrating on the problem in isolation (e.g., not considering changes in
player behavior) designers inadvertently created a positive feedback loop in which
players used their head and neck in increasingly risky ways. This resulted in more
injuries, which resulted in additional redesigns that made the helmet shells harder
and more padded, and so on.2
Negative feedback loops are effective for resisting change. For example, the
Segway Human Transporter uses negative feedback loops to maintain equilibrium.
As a rider leans forward or backward, the Segway accelerates or decelerates to
keep the system in equilibrium. To achieve this smoothly, the Segway makes
one hundred adjustments every second. Given the high adjustment rate, the
oscillations around the point of equilibrium are so small as to not be detectable.
However, if fewer adjustments were made per second, the oscillations would
increase in size and the ride would become increasingly jerky.
A key lesson of feedback loops is that things are connected—changing one
variable in a system will affect other variables in that system and other systems.
This is important because it means that designers must not only consider
particular elements of a design, but also their relation to the design as a whole
and the greater environment. Consider positive feedback loops to perturb systems
to change, but include negative feedback loops to prevent runaway behaviors that
lead to system failure. Consider negative feedback loops to stabilize systems, but
be cautious in that too much negative feedback in a system can lead to stagnation.3
See also Convergence, Errors, and Shaping.
1 In terms of practical application, the seminal
works on systems and feedback loops include
Industrial Dynamics, MIT Press, 1961;
Urban Dynamics, MIT Press, 1969 ; and
World Dynamics, MIT Press, 1970 , by
Jay W. Forrester.
2 See, for example, Why Things Bite Back:
Technology and the Revenge of Unintended
Consequences by Edward Tenner, Vintage
Books, 1997.
3 See, for example, Macroscope: A New
World Scientific System by Joel De Rosnay,
translated by Robert Edwards, Harper & Row
Publishers, 1979.
Feedback Loop

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Feedback Loop 93
The design history of the football
helmet is a classic example of positive
feedback. Positive feedback loops will
eventually collapse, or taper to an
Negative feedback loops are used
to stabilize systems—in this case,
to balance the Segway and its rider.
Negative feedback loops are applied
similarly in thermostatic systems and
S-shaped curve if limited by some other
factor, such as new rules penalizing the
use of helmets in tackling.
fly-by- wire controls in aircraft.
Negative feedback loops assume a
goal state, or oscillate around a goal
state if there are delays between the
variables in the loop.
Time
Hardness of Helmet
Injury Rate 	Player Risk-taking
	Performance
Positive Feedback Loop
Time
Angle of Segway 	Velocity
Performance
Negative Feedback Loop

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Feedback Loop** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Feedback Loop để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Convergence, Errors, and Shaping
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
