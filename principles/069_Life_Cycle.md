---
name: "Life Cycle"
vi: "Vòng đời sản phẩm (Life Cycle)"
summary: "Life Cycle (Vòng đời sản phẩm (Life Cycle)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Life Cycle (Vòng đời sản phẩm (Life Cycle))

> **Tóm tắt cốt lõi (Summary)**: Life Cycle là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Life Cycle
All products progress sequentially through four stages of
existence: introduction, growth, maturity, and decline.
All products progress through stages of existence that roughly correspond to birth,
life, and death. For example, a new type of electronic device is envisioned and
developed; its popularity grows; after a while its sales plateau; and then finally,
the sales decline. Understanding the implications of each of the stages allows
designers to prepare for the unique and evolving requirements of a product over
its lifetime. There are four basic stages of life for all products: introduction, growth,
maturity, and decline.1
Introduction
The introduction stage is the official birth of a product. It will at times overlap with
the late testing stage of the development cycle. The design focus is to monitor
early use of the design to ensure proper performance, working closely with
customers to tune or patch the design as necessary.
Growth
The growth stage is the most challenging stage, where most products fail. The
design focus is to scale the supply and performance of the product to meet the
growing demand, and provide the level of support necessary to maintain customer
satisfaction and growth. Efforts to gather requirements for the next-generation
product should be underway at this stage.
Maturity
The maturity stage is the peak of the product life cycle. Product sales have begun
to diminish and competition from competitors is strong. The design focus at this
stage is to enhance and refine the product to maximize customer satisfaction and
retention. Design and development of the next generation product should be well
underway at this stage.
Decline
The decline stage is the end of the life cycle. Product sales continue to decline
and core market share is at risk. The design focus is to minimize maintenance
costs and develop transition strategies to migrate customers to new products.
Testing of the next generation product should begin at this stage.
Consider the life cycle of a product when planning and preparing for the future.
During the introduction phase, work closely with early adopters to refine and tune
products. During the growth stage, focus on scaling product supply and performance.
During the maturity stage, focus on customer satisfaction through performance
enhancements and improved support. During decline, focus on facilitating the
transition to next generation products. Note that the development cycle for the next-
generation product begins during the growth stage of a current-generation product.
See also Development Cycle, Hierarchy of Needs, Iteration, and Prototyping.

1 The seminal work on the product life cycle is
“International Investment and International
Trade in the Product Cycle” by Raymond
Vernon, Quarterly Journal of Economics, 1966,
vol. 80, p. 190–207. A contemporary review
of the product life cycle is found in Marketing
Management by Philip Kotler, Prentice-Hall,
11th ed., 2002.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The needs of a product change
over the course of its life cycle. It is
important to understand the dynamics
of these changes in order to focus
business and design resources
accordingly. Failure to do so shortens
the life cycle of a product.
Life Cycle 151
Introduction 	Growth 	Maturity 	Decline
Audience 	Early Adopters 	Mainstream 	Late Adopters 	Laggards
Market 	Small 	Growing 	Large 	Contracting
Sales 	Low 	High 	Flattening 	Moderate
Competition 	Low 	Moderate 	High 	Moderate
Business Focus 	Awareness 	Market Share 	Customer Retention 	Transition
Design Focus 	Tuning 	Scaling 	Support 	Transition
Product Sales

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Life Cycle** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Life Cycle để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Development Cycle, Hierarchy of Needs, Iteration, and Prototyping
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
