---
name: "Prototyping"
vi: "Tạo mẫu thử nghiệm (Prototyping)"
summary: "Prototyping (Tạo mẫu thử nghiệm (Prototyping)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Prototyping (Tạo mẫu thử nghiệm (Prototyping))

> **Tóm tắt cốt lõi (Summary)**: Prototyping là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Prototyping
The use of simplified and incomplete models of a
design to explore ideas, elaborate requirements, refine
specifications, and test functionality.
Prototyping is the creation of simple, incomplete models or mockups of a design.
It provides designers with key insights into real-world design requirements,
and gives them a method to visualize, evaluate, learn, and improve design
specifications prior to delivery. There are three basic kinds of prototyping: concept,
throwaway, and evolutionary.1
Concept prototyping is useful for exploring preliminary design ideas quickly
and inexpensively. For example, concept sketches and storyboards are used
to develop the appearance and personality of characters in animated films well
before the costly process of animation and rendering take place. This approach
helps communicate the concepts to others, reveals design requirements and
problems, and allows for evaluation by a target audience. A common problem with
concept prototyping is the artificial reality problem, the plausible presentation of an
implausible design. A good artist or modeler can make most any design look like
it will work.
Throwaway prototyping is useful for collecting information about the functionality
and performance of certain aspects of a system. For example, models of new
automobile designs are used in wind tunnels to better understand and improve
the aerodynamics of their form. The prototypes are discarded once the needed
information is obtained. A common problem with throwaway prototyping is the
assumption that the functionality will scale or integrate properly in the final design,
which of course it often does not.
Evolutionary prototyping is useful when many design specifications are uncertain or
changing. In evolutionary prototyping, the initial prototype is developed, evaluated,
and refined continuously until it evolves into the final system. Design requirements
and specifications never define a final product, but merely the next iteration of the
design. For example, software developers invariably use evolutionary prototyping
to manage the rapid and volatile changes in design requirements. A common
problem with evolutionary prototyping is that designers tend to get tunnel vision,
focusing on tuning existing specifications, rather than exploring design alternatives.2
Incorporate prototyping into the design process. Use concept prototypes to develop
and evaluate preliminary ideas, and throwaway prototypes to explore and test
design functionalities and performance. Schedule time for prototype evaluation and
iteration. When design requirements are unclear or volatile, consider evolutionary
prototyping in lieu of traditional approaches. Consider the common problems
of artificial realities, scaling and integration, and tunnel vision when evaluating
prototypes and design alternatives.
See also Feedback Loop, Most Advanced Yet Acceptable, Satisficing, and
Scaling Fallacy.

1 See, for example, Human-Computer
Interaction by Jenny Preece, et al., Addison-
Wesley, 1994, p. 537–563; The Art of
Innovation by Tom Kelley and Jonathan
Littman, Doubleday, 2001; and Serious Play:
How the World’s Best Companies Simulate
to Innovate by Michael Schrage, Harvard
Business School Press, 1999.
2 Evolutionary prototyping is often contrasted
with incremental prototyping, which is the
decomposition of a design into multiple stages
that are then delivered one at a time. They are
combined here because they are invariably
combined in practice.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The function and elegance of the
Ojex Juicer clearly demonstrate the
benefits of prototyping in the design
process. Simple two-dimensional
prototypes were used to study
mechanical motion, three-dimensional
foam prototypes were used to study
form and assembly, and functional
breadboard models were used to
study usability and working stresses.
Prototyping 195

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Prototyping** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Prototyping để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Feedback Loop, Most Advanced Yet Acceptable, Satisficing, and
Scaling Fallacy
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
