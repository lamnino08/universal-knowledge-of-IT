---
name: "Hierarchy of Needs"
vi: "Thang bậc nhu cầu thiết kế"
summary: "Hierarchy of Needs (Thang bậc nhu cầu thiết kế): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Hierarchy of Needs (Thang bậc nhu cầu thiết kế)

> **Tóm tắt cốt lõi (Summary)**: Hierarchy of Needs là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Hierarchy of Needs
In order for a design to be successful, it must meet
people’s basic needs before it can attempt to satisfy
higher-level needs.1
The hierarchy of needs principle specifies that a design must serve the low-level
needs (e.g., it must function), before the higher-level needs, such as creativity,
can begin to be addressed. Good designs follow the hierarchy of needs principle,
whereas poor designs may attempt to meet needs from the various levels without
building on the lower levels of the hierarchy first. The five key levels of needs in
the hierarchy are described below.2
Functionality needs have to do with meeting the most basic design requirements.
For example, a video recorder must, at minimum, provide the capability to record,
play, and rewind recorded programs. Designs at this level are perceived to be of
little or no value.
Reliability needs have to do with establishing stable and consistent performance.
For example, a video recorder should perform consistently and play back recorded
programs at an acceptable level of quality. If the design performs erratically, or is
subject to frequent failure, reliability needs are not satisfied. Designs at this level
are perceived to be of low value.
Usability needs have to do with how easy and forgiving a design is to use. For
example, configuring a video recorder to record programs at a later time should be
easily accomplished, and the recorder should be tolerant of mistakes. If the difficulty
of use is too great, or the consequences of simple errors too severe, usability needs
are not satisfied. Designs at this level are perceived to be of moderate value.
Proficiency needs have to do with empowering people to do things better than
they could previously. For example, a video recorder that can seek out and record
programs based on keywords is a significant advance in recording capability,
enabling people to do things not previously possible. Designs at this level are
perceived to be of high value.
Creativity is the level in the hierarchy where all needs have been satisfied, and
people begin interacting with the design in innovative ways. The design, having
satisfied all other needs, is now used to create and explore areas that extend both
the design and the person using the design. Designs at this level are perceived to
be of the highest value, and often achieve cult-like loyalty among users.
Consider the hierarchy of needs in design, and ensure that lower-level needs are
satisfied before resources are devoted to serving higher-level needs. Evaluate
existing designs with respect to the hierarchy to determine where modifications
should be made.
See also 80/20 Rule, Aesthetic-Usability Effect, and Form Follows Function.

1 The hierarchy of needs is based on Maslow’s
Hierarchy of Needs.
2 The seminal work on the concept of a
hierarchy of needs is Motivation and
Personality by Abraham Maslow, Addison-
Wesley, 1987 [1954].

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Hierarchy of Needs 125
The hierarchy of needs specifies that
a design must address lower-level
needs before higher-level needs can
be addressed. The perceived value
of a design corresponds to its place
in the hierarchy—i.e., higher levels
in the hierarchy correspond to higher
levels of perceived value. The levels of
hierarchy are adapted from Maslow’s
Hierarchy of Needs.
Maslow’s Hierarchy of Needs
Hierarchy of Needs
Creativity
Proficiency
Usability
Reliability
Functionality
Self-Actualization
Self-Esteem
Love
Safety
Physiological

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Hierarchy of Needs** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Hierarchy of Needs để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Aesthetic-Usability Effect, and Form Follows Function
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
