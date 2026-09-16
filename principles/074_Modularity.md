---
name: "Modularity"
vi: "Tính mô-đun hóa (Modularity)"
summary: "Modularity (Tính mô-đun hóa (Modularity)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Modularity (Tính mô-đun hóa (Modularity))

> **Tóm tắt cốt lõi (Summary)**: Modularity là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Modularity
A method of managing system complexity that involves
dividing large systems into multiple, smaller self-
contained systems.
Modularity is a structural principle used to manage complexity in systems.
It involves identifying functional clusters of similarity in systems, and then
transforming the clusters into interdependent self-contained systems (modules).
For example, the modular design of computer memory chips provides computer
owners the option of increasing the memory in their computer without any
requirement to do so. If the design of the computer and memory chips were not
modular in this way, the only practical method of upgrading computer memory
would be to buy a new computer. The option to easily and inexpensively improve
a system without the requirement to do so gives modular designs an intrinsic
advantage over non-modular designs.1
Modules should be designed to hide their internal complexity and interact with
other modules through simple interfaces. The result is an overall reduction
in system complexity and a decentralization of system architecture, which
improves reliability, flexibility, and maintainability. Additionally, a modular design
encourages innovation of modules, as well as competition regarding their design
and manufacture; it creates an opportunity for third parties to compete to develop
better modules.
The benefits of modular design are not without costs: modular systems are
significantly more complex to design than nonmodular systems. Designers must
have significant knowledge of the inner workings of a system and its environment
to decompose the systems into modules, and then make those modules function
together as a whole. Consequently, most modular systems that exist today did not
begin that way—they have been incrementally transformed to be more modular
as knowledge of the system increased.
Consider modularity when designing or modifying complex systems. Identify
functional clusters of similarity in systems, and clearly define their relationships
with other system elements. If feasible, create modules that conceal their
complexity and communicate with other modules through simple, standard
interfaces. Do not attempt complex modular designs without experienced
designers and a thorough understanding of the system. However, consider the
incremental modularization of existing systems, especially during maintenance
and product updates.2
See also 80/20 Rule, Chunking, and Cost-Benefit.

1 The seminal work on modularity is Design
Rules: Volume I. The Power of Modularity
by Carliss Y. Baldwin and Kim B. Clark, MIT
Press, 2000.
2 Many designers resist modularity for fear of
limiting creativity. However, modules applied
at the appropriate level will liberate designers
from useless activity and allow them to focus
creativity where it is most needed.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The rapid increase in availability,
quality, and computing power of
personal computers over the last
twenty years is largely attributable
to their modular designs. The key
components of the computer are
standard modules that use standard
interfaces. This enables competition
among third-party manufacturers to
improve modules and reduce price,
which also improves the computer
and reduces its price.
Modularity 161
Personal Computer
Power Supply
Graphics Card
Sound Card
CD-ROM Drive
Hard Drive
Memory
Processor
CPU
Floppy Drive

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Modularity** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Modularity để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Chunking, and Cost-Benefit
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
