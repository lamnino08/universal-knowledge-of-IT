---
name: "Hick’s Law"
vi: "Định luật Hick"
summary: "Hick’s Law (Định luật Hick): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Hick’s Law (Định luật Hick)

> **Tóm tắt cốt lõi (Summary)**: Hick’s Law là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Hick’s Law
The time it takes to make a decision increases as the
number of alternatives increases.1
Hick’s Law states that the time required to make a decision is a function of the
number of available options. It is used to estimate how long it will take for people
to make a decision when presented with multiple choices. For example, when
a pilot has to press a particular button in response to some event, such as an
alarm, Hick’s Law predicts that the greater the number of alternative buttons, the
longer it will take to make the decision and select the correct one. Hick’s Law has
implications for the design of any system or process that requires simple decisions
to be made based on multiple options.2
All tasks consist of four basic steps: (1) identify a problem or goal, (2) assess the
available options to solve the problem or achieve the goal, (3) decide on an option,
and (4) implement the option. Hick’s Law applies to the third step: decide on an
option. However, the law does not apply to decisions that involve significant levels
of searching, reading, or complex problem solving. For example, a complex task
requiring reading sentences and intense concentration with three options can
easily take longer than a simple stimulus-response task with six options. Therefore,
Hick’s Law is most applicable for simple decision-making tasks in which there is a
unique response to each stimulus. For example, if A happens, then push button
1, If B happens, then push button 2. The law is decreasingly applicable as the
complexity of tasks increases.3
Designers can improve the efficiency of a design by understanding the
implications of Hick’s Law. For example, the law applies to the design of software
menus, control displays, wayfinding layout and signage, and emergency response
training—as long as the decisions involved are simple. As the complexity of the
tasks increases, the applicability of Hick’s Law decreases. For example, Hick’s
Law does not apply to complex menus or hierarchies of options. Menu selection
of this type is not a simple decision-making task since it typically involves reading
sentences, searching and scanning for options, and some level of problem solving.
Consider Hick’s Law when designing systems that involve decisions based on a set
of options. When designing for time-critical tasks, minimize the number of options
involved in a decision to reduce response times and minimize errors. When
designs require complex interactions, do not rely on Hick’s Law to make design
decisions; rather, test designs on the target population using realistic scenarios.
In training people to perform time-critical procedures, train the fewest possible
responses for a given scenario. This will minimize response times, error rates, and
training costs.
See also Errors, Fitts’ Law, Progressive Disclosure, and Wayfinding.
1 Also known as Hick-Hyman Law.
2 The seminal work on Hick’s Law is “On the
Rate of Gain of Information” by W. E. Hick,
Quarterly Journal of Experimental Psychology,
1952, vol. 4, p. 11–26; and “Stimulus
information as a determinant of reaction
time” by Ray Hyman, Journal of Experimental
Psychology, 1953, vol. 45, p. 188–196.
3 The Hick’s Law equation is RT = a + b log 2
(n), where RT = response time, a = the total
time that is not involved with decision making,
b = an empirically derived constant based on
the cognitive processing time for each option
(in this caseࠪ  	0.155 seconds for humans), n
= number of equally probable alternatives. For
example, assume it takes 2 seconds to detect
an alarm and understand it’s meaning. Further,
assume that pressing one of five buttons will
solve the problem caused by the alarm. The
time to respond would be RT = (2 sec) +
(0.155 sec)(log 2 (5)) = 2.36 sec.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

File
New ...
Open
Open Recent Files
Revert
Close
Save
Save As ...
Save a Copy ...
Save for Web ...
NORTH
TO
TO
EAST
NORTH
TO
WEST
TO
SOUTH
TO
Menus
The time for a person to select an
item from a simple software menu
increases with the number of items.
However, this may not be the case for
more complex menus involving a lot of
text or submenus.
Predatory Behavior
The time for a predator to target a
prey increases with the number of
potential prey.
Simple Tasks
The time for a person to press the
correct button (R, G, or B) depending
on the color of the light (red, green,
or blue) increases with the number of
possible colors.
Test Options
Hick’s Law does not apply to tasks
involving significant levels of reading
and problem solving, as in taking
an exam.
Device Settings
The time for a person to make simple
decisions about adjustments on a
device increases with the number
of controls. This may not be the
case for more complex decisions or
combinations of settings.
Martial Arts
The time for a martial artist to block a
punch increases with the number of
known blocking techniques.
Braking
The time for a driver to press the
brake to avoid hitting an unexpected
obstacle increases if there is a clear
opportunity to steer around the
obstacle.
Road Signs
As long as road signs are not too
dense or complex, the time for a driver
to make a turn based on a particular
road sign increases with the total
number of road signs.
Hick’s Law 121

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Hick’s Law** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Hick’s Law để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Errors, Fitts’ Law, Progressive Disclosure, and Wayfinding
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
