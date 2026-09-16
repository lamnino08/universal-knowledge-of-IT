---
name: "Development Cycle"
vi: "Chu kỳ phát triển sản phẩm"
summary: "Development Cycle (Chu kỳ phát triển sản phẩm): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Development Cycle (Chu kỳ phát triển sản phẩm)

> **Tóm tắt cốt lõi (Summary)**: Development Cycle là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Successful products typically follow four stages of
creation: requirements, design, development, and testing.
All products progress sequentially through basic stages of creation. Understanding
and using effective practices for each stage allows designers to maximize a
product’s probability of success. There are four basic stages of creation for all
products: requirements, design, development, and testing. 1
Requirements
In formal processes, requirements are gathered through market research, customer
feedback, focus groups, and usability testing. Informally, design requirements are
often derived from direct knowledge or experience. Design requirements are best
obtained through controlled interactions between designers and members of the
target audience, and not simply by asking people what they want or like—often
they do not know, or cannot clearly articulate their needs.
Design
This stage is where design requirements are translated into a form that yields a set
of specifications. The goal is to meet the design requirements, though an implicit
goal is to do so in a unique fashion. Excellent design is usually accomplished
through careful research of existing or analogous solutions, active brainstorming
of many diverse participants, ample use of prototyping, and many iterations of
trying, testing, and tuning concepts. A design that is appreciably the same at the
beginning and end of this stage is probably not much of a design.
Development
The development stage is where design specifications are transformed into an actual
product. The goal of development is to precisely meet the design specifications. Two
basic quality control strategies are used to accomplish this: reduce variability in the
materials, creations of parts, and assembly of parts; and verify that specifications are
being maintained throughout the development process.
Testing
The testing stage is where the product is tested to ensure that it meets design
requirements and specifications, and will be accepted by the target audience.
Testing at this stage generally focuses on the quality of modules and their
integration, real-world performance (real contexts, real users), and ease and
reliability of installation.
Gather requirements through controlled interactions with target audiences,
rather than simple feedback or speculation by team members. Use research,
brainstorming, prototyping, and iterative design to achieve optimal designs.
Minimize variability in products and processes to improve quality. Test all aspects
of the design to the degree possible.
See also Design by Committee, Hierarchy of Needs, Iteration, Life Cycle, and
Prototyping
1 A nice treatment of contemporary product
development issues and strategies is found
in Products in Half the Time: New Rules,
New Tools by Preston G. Smith and Donald
G. Reinertsen, John Wiley & Sons, 2nd ed.,
1997; and Managing the Design Factory: The
Product Developer’s Toolkit by Donald G.
Reinertsen, Free Press, 1997.
78
Development Cycle

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

0%
100%
0%
100%
Althoughprogress throughthe
development cycle is sequential, it can
be linear or iterative.The linear model
(also known as the 	waterfall model)
proceeds through the development
cycle once, completing each stage
before proceeding to the next. The
iterative model (also known as the
spiral model) proceeds through the
development cycle multiple times,
completing an increasing percentage
of each stage with each iteration.
The linear model is preferred when
requirements and specifications are
exact and unchanging, and the cost
of iteration is prohibitive. In all other
cases, the iterative model is preferred.
Development Cycle 79
Linear
Requirements
Design
Development
Testing
Time
Iterative
Requirements
Design
Development
Testing
Time

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Development Cycle** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Development Cycle để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Design by Committee, Hierarchy of Needs, Iteration, Life Cycle, and
Prototyping
1 A nice treatment of contemporary product
development issues and strategies is found
in Products in Half the Time: New Rules,
New Tools by Preston G
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
