---
name: "Satisficing"
vi: "Thỏa mãn vừa đủ (Satisficing)"
summary: "Satisficing (Thỏa mãn vừa đủ (Satisficing)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Satisficing (Thỏa mãn vừa đủ (Satisficing))

> **Tóm tắt cốt lõi (Summary)**: Satisficing là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

1 Also known as best is the enemy of the
good principle.
2 The seminal works on satisficing are Models
of Man, John Wiley & Sons, 1957; and The
Sciences of the Artificial, MIT Press, 1969, both
by Herbert A. Simon.
3 In many time-limited contexts, the time limits
are artificial (i.e., set by management), whereas
the consequences of low-quality design and
system failure are real. See, for example,
Crucial Decisions: Leadership in Policymaking
and Crisis Management by Irving Janis, Free
Press, 1989.
4 For example, designers at Swatch realized
that watches of increasing accuracy were no
longer of value to consumers—i.e., accuracy to
within one minute a day was accurate enough.
This “good enough” standard allowed the
designers of Swatch to focus their efforts on
style and cost reduction, rather than on further
optimizing the timekeeping of their watches.

Satisficing
It is often preferable to settle for a satisfactory solution,
rather than pursue an optimal solution.1
The best design decision is not always the optimal design decision. In certain
circumstances, the success of a design is better served by design decisions that
roughly satisfy (i.e., satisfice), rather than optimally satisfy, design requirements.
For example, in seeking for the proverbial needle in a haystack, a satisficer would
stop looking as soon as a needle is found; an optimizer would continue to look for
all possible needles so that the sharpest needle could be determined. There are
three kinds of problems for which satisficing should be considered: very complex
problems, time-limited problems, and problems for which anything beyond a
satisfactory solution yields diminishing returns.2
Complex design problems are characterized by a large number of interacting
variables and a large number of unknowns. In working with such problems, a
satisficer recognizes that the combination of complexity and unknowns makes
an optimal solution unlikely (if not impossible). The satisficer, therefore, seeks a
satisfactory solution that is just better than existing alternatives; the satisficer seeks
only to incrementally improve upon the current design, rather than to achieve an
optimal design.
Time-limited problems are characterized by time frames that do not permit
adequate analysis or development of an optimal solution. In cases where optimality
is secondary to urgency, a satisficer selects the first solution that satisfactorily meets
a given design requirement. Note that satisficing should be cautiously applied in
time-limited contexts, especially when the consequences of a suboptimal solution
can have serious consequences.3
There are cases in which a satisfactory solution is better than an optimal solution—
i.e., solutions beyond the satisfactory yield diminishing returns. Determining when
satisfactory is best requires accurate knowledge of the design requirements, and
accurate knowledge of the value perceptions of the users. A satisficer weighs this
value perception in the development of the design specification, ensuring that
optimal specifications will not consume design resources unless they are both
critical to success, and accorded value by users.4
Consider satisficing as a means of making design decision when problems are
complex with many unknowns, when problems need to be solved within a narrow
time frame, and when developing design requirements and specifications. Generally,
do not accept satisficed solutions that are inferior to previous or existing solutions.
In time-limited contexts, consider satisficing only when the limited timelines are
truly fixed, and the consequences of low-quality design and increased risk of
failure are acceptable.
See also 80/20 Rule, Chunking, Cost-Benefit, Iteration, and Not Invented Here.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The adapted square carbon dioxide
filter from the command module
(center), and round filter receptacle of
the lunar lander (lower right).
Astronaut John L. Swigert Jr., hooking
up the adapted carbon dioxide filters.
The Apollo 13 Mission to the moon
launched at 2:13 P.M. EST on
April 11, 1970. An electrical failure
occurred in the command module
of the spacecraft 56 hours into
the flight, causing the mission to
be aborted and forcing the three-
person crew to take refuge in the
lunar lander. The carbon dioxide
filters aboard the lunar lander were
designed to support two people for
two days—the planned duration
of a lunar landing—and not the
three people for four days needed
to return the crew safely to Earth.
The square carbon dioxide filters of
the abandoned command module
had the capacity to filter the excess
carbon dioxide, but did not fit into
the round filter receptacle of the lunar
lander. Using materials available
on the spacecraft such as plastic
bags, cardboard from log books,
and duct tape, NASA engineers
designed a makeshift adapter for the
square command module filters. The
ground crew talked the astronauts
through the construction process,
and the adapted filters were put into
service immediately thereafter. The
solution was far from optimal, but it
was satisfactory—it eliminated the
immediate danger of carbon dioxide
poisoning, and allowed ground and
flight crews to focus on other critical
problems. The crew of Apollo 13
returned safely home at 1:07 P.M. EST
on April 17, 1970.
Satisficing 211

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Satisficing** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Satisficing để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Chunking, Cost-Benefit, Iteration, and Not Invented Here
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
