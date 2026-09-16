---
name: "Consistency"
vi: "Tính nhất quán (Consistency)"
summary: "Consistency (Tính nhất quán (Consistency)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - usability
---

# Universal Design Principle: Consistency (Tính nhất quán (Consistency))

> **Tóm tắt cốt lõi (Summary)**: Consistency là một nguyên lý thiết kế then chốt thuộc nhóm **perception, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The usability of a system is improved when similar parts
are expressed in similar ways.
According to the principle of consistency, systems are more usable and learnable
when similar parts are expressed in similar ways. Consistency enables people to
efficiently transfer knowledge to new contexts, learn new things quickly, and focus
attention on the relevant aspects of a task. There are four kinds of consistency:
aesthetic, functional, internal, and external.1
Aesthetic consistency refers to consistency of style and appearance (e.g.,
a company logo that uses a consistent font, color, and graphic). Aesthetic
consistency enhances recognition, communicates membership, and sets
emotional expectations. For example, Mercedes-Benz vehicles are instantly
recognizable because the company consistently features its logo prominently
on the hood or grill of its vehicles. The logo has become associated with quality
and prestige, and informs people how they should feel about the vehicle—i.e.,
respected and admired.
Functional consistency refers to consistency of meaning and action (e.g., a
traffic light that shows a yellow light before going to red). Functional consistency
improves usability and learnability by enabling people to leverage existing
knowledge about how the design functions. For example, videocassette recorder
control symbols, such as for rewind, play, forward, are now used on devices
ranging from slide projectors to MP3 music players. The consistent use of these
symbols on new devices enables people to leverage existing knowledge about how
the controls function, which makes the new devices easier to use and learn.
Internal consistency refers to consistency with other elements in the system
(e.g., signs within a park are consistent with one another). Internal consistency
cultivates trust with people; it is an indicator that a system has been designed, and
not cobbled together. Within any logical grouping elements should be aesthetically
and functionally consistent with one another.
External consistency refers to consistency with other elements in the environment
(e.g., emergency alarms are consistent across different systems in a control room).
External consistency extends the benefits of internal consistency across multiple,
independent systems. It is more difficult to achieve because different systems
rarely observe common design standards.
Consider aesthetic and functional consistency in all aspects of design. Use
aesthetic consistency to establish unique identities that can be easily recognized.
Use functional consistency to simplify usability and ease of learning. Ensure that
systems are always internally consistent, and externally consistent to the greatest
degree possible. When common design standards exist, observe them.
See also Modularity, Recognition Over Recall, and Similarity.

1 Use consistent approaches when possible,
but do not compromise clarity or usability
for consistency. In the words of Emerson,
“A foolish consistency is the hobgoblin of
little minds …”
Consistency

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Restaurant chains frequently use
consistency to provide customers with
the same experience across many
locations. For example, Bob Evans
uses the same logo, typefaces, color
schemes, menus, staff uniforms,
interior design, and architecture
across its restaurants. This consistency
improves brand recognition, reduces
costs, and establishes a relationship
with customers that extends beyond
any single restaurant.
Consistency 57

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Consistency** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Consistency để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Modularity, Recognition Over Recall, and Similarity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
