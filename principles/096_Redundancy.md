---
name: "Redundancy"
vi: "Dự phòng và dư thừa (Redundancy)"
summary: "Redundancy (Dự phòng và dư thừa (Redundancy)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Redundancy (Dự phòng và dư thừa (Redundancy))

> **Tóm tắt cốt lõi (Summary)**: Redundancy là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Redundancy
The use of more elements than necessary to maintain the
performance of a system in the event of failure of one or
more of the elements.
System failure is the failure of a system to achieve a goal—e.g., communicate a
message, maintain a structural load, or maintain operation. It is inevitable that
elements within a system will fail. It is not inevitable, however, that the system as a
whole fails. Redundancy is the surest method of preventing system failure. There
are four kinds of redundancy: diverse, homogenous, active, and passive.1
Diverse redundancy is the use of multiple elements of different types (e.g., use
of text, audio, and video to present the same information). Diverse redundancy is
resistant to a single cause of failure, but is complex to implement and maintain.
For example, high-speed trains often have diverse redundancy in their braking
systems—one electric brake, one hydraulic brake, and one pneumatic brake. A
single cause is unlikely to result in a cascade failure in all three braking systems.
Homogenous redundancy is the use of multiple elements of a single type (e.g.,
use of multiple independent strands to compose a rope). Homogenous redun-
dancy is relatively simple to implement and maintain but is susceptible to single
causes of failure—i.e., the type of cause that results in failure in one element
can result in failure of other redundant elements. For example, a sharp edge that
severs one strand of a rope can sever others.
Active redundancy is the application of redundant elements at all times (e.g.,
using multiple independent pillars to support a roof). Active redundancy guards
against both system and element failure—i.e., it distributes loads across all
elements such that the load on the each element and the overall system
is reduced. Active redundancy also allows for element failure, repair, and
substitution with minimal disruption of system performance.
Passive redundancy is the application of redundant elements only when an
active element fails (e.g., using a spare tire on a vehicle in the event of a flat tire).
Passive redundancy is ideal for noncritical elements, but it will result in system
failure when used for elements critical to system operation. Passive redundancy is
the simplest and most common kind of redundancy.
Use diverse redundancy for critical systems when the probable causes of failure
cannot be anticipated. Use homogenous redundancy when the probable causes
of failure can be anticipated. Use active redundancy for critical systems that must
maintain stable performance in the event of element failure or extreme changes
in system load. Use passive redundancy for noncritical elements within systems,
or systems in which performance interruptions are tolerable. The four kinds of
redundancy should be used in combination to achieve highly reliable systems.
See also Factor of Safety, Modularity, Structural Forms, and Weakest Link.

1 See, for example, Why Buildings Fall Down:
How Structures Fail by Matthys Levy and Mario
Salvadori, W.W. Norton, 1992; and “Achieving
Reliability: The Evolution of Redundancy in
American Manned Spacecraft” by James E.
Tomayko, Journal of the British Interplanetary
Society, 1985, vol. 38, p. 545–552.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Redundancy 205
Parts 	Purpose
1 fiberglass cow 	protect the city from danger
1 canvas cape 	flap in the wind
1 tower crane 	provide a bovine perch
1 fabricated steel base 	display cow above crane railings
4 fabricated steel hoof plates 	attach cow to base
2 steel cables 	attach cow to base
8 bolts 	attach hoof plates to base
1 steel cross member 	attach base to crane
2 fabricated double U-bolts 	attach cross member to base
2 steel guy wires 	attach base to crane
3 eyebolts 	attach cape to cow
Eyebolts
Canvas Cape
Steel Cables
(Inside Cow)
Bolts
Guy Wire 	Guy Wire
Steel Cross Member
Tower Crane
Fabricated
Steel Base
Fabricated
Steel Hoof Plates
Fabricated Double U-Bolts
Fiberglass Cow
The Super Cow entry in the Houston
Cow Parade 2001 had a unique
design specification—it was to sit
atop a thirty-story tower crane for the
duration of hurricane season. Since
the consequences of Super Cow
taking flight in high winds could be
grave, various forms of redundancy
were applied to keep him attached.
Despite many severe thunderstorms
(wind gusts in excess of 60 MPH),
Super Cow experienced no failure,
damage, or unintended flights during
his four-month stay on the crane.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Redundancy** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Redundancy để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Factor of Safety, Modularity, Structural Forms, and Weakest Link
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
