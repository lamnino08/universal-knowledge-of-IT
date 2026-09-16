---
name: "Factor of Safety"
vi: "Hệ số an toàn (Factor of Safety)"
summary: "Factor of Safety (Hệ số an toàn (Factor of Safety)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Factor of Safety (Hệ số an toàn (Factor of Safety))

> **Tóm tắt cốt lõi (Summary)**: Factor of Safety là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The use of more elements than is thought to be necessary
to offset the effects of unknown variables and prevent
system failure.1
Design requires dealing with unknowns. No matter how knowledgeable the designer
and how thoroughly researched the design specification, basic assumptions about
unknowns of one kind or another are inevitable in every design process. Factors of
safety are used to offset the potential effects of these unknowns. This is achieved
by adding materials and components to the system in order to make the design
exceed the specification that is believed to be necessary to meet the design
requirements. For example, designing an Internet service that can support one
thousand users is straightforward. However, to account for unanticipated uses of
the service (e.g., downloading large files), the design specification can be multiplied
by a safety factor (e.g., three). In this case, a safety factor of three would mean that
the service would be rated to support one thousand users, but actually designed to
support three times that many, or three thousand users.
The size of the safety factor corresponds directly to the level of ignorance of the
design parameters. The greater the ignorance, the greater the safety factor. For
example, structures that are well understood and made of materials of consistent
quality, such as steel and concrete structures, typically use a safety factor ranging
from two to four. Structures that are well understood and made of materials of
varying quality, such as wood, may use a safety factor ranging from four to eight.
When ignorance is combined with materials of varying quality, the safety factor
can get quite large. For example, the designers of the Great Pyramid at Giza
unknowingly applied a safety factor of over twenty.2
Increasing the safety factor in a design translates into the addition of elements
(e.g., materials). More elements means more cost. New designs must typically
have large factors of safety because the number of unknowns is great. If a design
performs reliably over time, confidence that the unknowns in the system have
been managed combines with the pressure to reduce costs, and typically leads to
a “tuning” process to reduce elements and lower the safety factor. Unfortunately,
this process usually continues until an accident or failure occurs, at which point
cost considerations become secondary and safety factors are again increased.3
Use safety factors to minimize the probability of failure in a design. Apply them
in proportion to the ignorance of the design parameters and the severity of the
consequences of failure. Reduce safety factors with caution, especially when
specifications extend beyond design precedents. Observe the rated capacity of
a system when making decisions that stress system limits, and not the designed
capacity (capacity including factors of safety), except in cases of emergency.
See also Design by Committee, Errors, Modularity, Structural Forms, and
Weakest Link.
1 Also known as factor of ignorance.
2 Note that different elements within a system
can observe different factors of safety. For
example, a wing on an aircraft may apply a
factor of safety that is much greater than the
factor of safety applied to less critical elements.
3 See, for example, To Engineer Is Human:
The Role of Failure in Successful Design,
Macmillan, 1985; and Design Paradigms:
Case Histories of Error and Judgment in
Engineering, Cambridge University Press,
1994, both by Henry Petroski.
Factor of Safety

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1981 	1986	1985	1984	1983	1982
1
2
3
20
40
60
80
100
The O-ring design of the space shuttle
Challenger’s solid rocket booster was
designed to have a safety factor of
three. However, low temperatures
contributed to the erosion of O-rings
in past launches and, consequently,
to the erosion of this safety factor; at
low temperatures, the safety factor
was well below three. On the morning
of January 28, 1986, the temperature
at the launch pad was 36 degrees F
(2.2 degrees C)—the lowest launch
temperature to date. Despite the
objections of several engineers, the
decision to proceed with the launch
was based largely on the belief that
the safety factor was sufficient to
offset any low-temperature risks.
Catastrophic failure occurred shortly
after launch.
Factor of Safety 91
Factor of Safety
Temperature (°F)
Shuttle Launches
No O-ring damage
Minor O-ring damage
Major O-ring damage
Rubber O-rings, about 38 feet (11.6 meters)
in circumference and 1
⁄4 inch (0.635 cm) thick.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Factor of Safety** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Factor of Safety để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Design by Committee, Errors, Modularity, Structural Forms, and
Weakest Link
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
