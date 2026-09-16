---
name: "Visibility"
vi: "Tính hiển thị rõ ràng (Visibility)"
summary: "Visibility (Tính hiển thị rõ ràng (Visibility)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - usability
---

# Universal Design Principle: Visibility (Tính hiển thị rõ ràng (Visibility))

> **Tóm tắt cốt lõi (Summary)**: Visibility là một nguyên lý thiết kế then chốt thuộc nhóm **perception, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Visibility
The usability of a system is improved when its status and
methods of use are clearly visible.
According to the principle of visibility, systems are more usable when they
clearly indicate their status, the possible actions that can be performed, and the
consequences of the actions once performed. For example, a red light could be
used to indicate whether or not a device is receiving power; illuminated controls
could be used to indicate controls that are currently available; and distinct
auditory and tactile feedback could be used to acknowledge that actions have
been performed and completed. The principle of visibility is based on the fact that
people are better at recognizing solutions when selecting from a set of options,
than recalling solutions from memory. When it comes to the design of complex
systems, the principle of visibility is perhaps the most important and most violated
principle of design.1
To incorporate visibility into a complex system, one must consider the number
of conditions, number of options per condition and number of outcomes—the
combinations can be overwhelming. This leads many designers to apply a type of
kitchen-sink visibility—i.e., they try to make everything visible all of the time. This
approach may seem desirable, but it actually makes the relevant information and
controls more difficult to access due to an overload of information.2
Hierarchical organization and context sensitivity are good solutions for managing
complexity while preserving visibility. Hierarchical organization puts controls and
information into logical categories, and then hides them within a parent control,
such as a software menu. The category names remain visible, but the controls
and information remain concealed until the parent control is activated. Context
sensitivity reveals and conceals controls and information based on different
system contexts. Relevant controls and information for a particular context are
made highly visible, and irrelevant controls (e.g., unavailable functions), are
minimized or hidden.
Visible controls and information serve as reminders for what is and is not possible.
Design systems that clearly indicate the system status, the possible actions that
can be performed, and the consequences of the actions performed. Immediately
acknowledge user actions with clear feedback. Avoid kitchen-sink visibility. Make
the degree of visibility of controls and information correspond to their relevance.
Use hierarchical organization and context sensitivity to minimize complexity and
maximize visibility.
See also Affordance, Mapping, Mental Model, Modularity, Progressive Disclosure,
and Recognition Over Recall.

1 The seminal work on visibility is The Design
of Everyday Things by Donald Norman,
Doubleday, 1990.
2 The enormity of the number of visibility
conditions is why visibility is among the most
violated of the design principles—it is, quite
simply, difficult to accommodate all of the
possibilities of complex systems.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

00:00:00
00:00:02
00:00:03
00:00:04
00:00:09
00:00:11
00:02:00
00:04:30
00:08:00
01:20:00
01:40:00
02:15:00
02:20:00
02:45:00
07:30:00
09:00:00
15:00:00
6
1
2
2A
3
4
5
7
2
1
1
1
3
2A
2A
4
5
7
3 7
3 4
3 7
7
3 5 7
3 7
3
6
7
7
2A 7
7
5 7
TIME 	PLACE 	EVENT
Visibility 251
Three Mile Island Unit 2
Harrisburg, Pennsylvania
March 28, 1979, 4:00 A.M.
Secondary Loop
Primary Loop
Control Room
Visibility of complex systems is essential
for problem solving—especially in
times of stress. An analysis of key
events of the TMI accident reveals a
number of blind spots in the system
that made understanding and solving
the problems exceedingly difficult.
To further complicate matters, alarms
were blaring, lights were flashing, and
critical system feedback was routed
to a printer that could only print
15 lines a minute—status information
was more than an hour behind for
much of the crisis.
Coolant pumps in the secondary loop malfunction and shut down.
Temperature and pressure in the primary loop increase.
The pressure release valve (PORV) opens automatically to lower the pressure.
Backup pumps automatically turn on.
Operators do not know that the backup pumps are disconnected.
The control rods are lowered to slow the nuclear chain reaction and reduce the temperature.
The PORV light goes out in the control room, indicating that the PORV closed.
Operators cannot see that the PORV is stuck open. Steam and water is released through the PORV.
Emergency water is automatically injected into the primary loop to keep the water at a safe level.
Instruments in the control room indicate that water level in the primary loop is rising. Operators shut down
the emergency water injection.
Operators cannot see that the water level in the primary loop is actually dropping. Steam and water
continue to be released through the PORV.
An operator notices that the backup pumps are not working. He connects the pumps and they begin
operating normally.
Pumps in the primary loop vibrate violently because of steam in the line. Two of four pumps are shut down.
The other two pumps shut down. Temperature and pressure in the primary loop continue to rise.
The water level drops below the core. Radioactive gas is released through the PORV.
An operator notices that the temperature at the PORV is high. He stops the leak by shutting a PORV
backup valve.
Operators still cannot see that the water level in the primary loop is actually dropping.
Radiation alarms sound and a site emergency is declared. The level of radioactivity in the primary loop is
over 300 times the normal level.
Operators pump water into the primary loop, but cannot bring the pressure down. They open the backup valve
to the PORV to lower pressure.
An explosion occurs in the containment structure.
Operators cannot see that an explosion occurred. They attribute the noise and instrument readings to an
electrical malfunction.
The pumps in the primary loop are reactivated. Temperatures decline and the pressure lowers. Disaster is
averted—except, of course, for the leaking radiation.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Visibility** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Visibility để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Mapping, Mental Model, Modularity, Progressive Disclosure,
and Recognition Over Recall
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
