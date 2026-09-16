---
name: "Uncertainty Principle"
vi: "Nguyên lý bất định (Uncertainty Principle)"
summary: "Uncertainty Principle (Nguyên lý bất định (Uncertainty Principle)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Uncertainty Principle (Nguyên lý bất định (Uncertainty Principle))

> **Tóm tắt cốt lõi (Summary)**: Uncertainty Principle là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Uncertainty Principle
The act of measuring certain sensitive variables in a
system can alter them, and confound the accuracy of
the measurement.
This principle is based on Heisenberg’s uncertainty principle in physics.
Heisenberg’s uncertainty principle states that both the position and momentum of
an atomic particle cannot be known because the simple act of measuring either
one of them affects the other. Similarly, the general uncertainty principle states
that the act of measuring sensitive variables in any system can alter them, and
confound the accuracy of the measurement. For example, a common method of
measuring computer performance is event logging: each event that is performed
by the computer is recorded. Event logging increases the visibility of what the
computer is doing and how it is performing, but it also consumes computing
resources, which interferes with the performance being measured.
The uncertainty introduced by a measure is a function of the sensitivity of
variables in a system, and the invasiveness of the measure. Sensitivity refers to
the ease with which a variable in a system is altered by the measure. Invasiveness
refers to the amount of interference introduced by the measure. Generally, the
invasiveness of the measure should be inversely related to the sensitivity of the
variable measured; the more sensitive the variable, the less invasive the measure.
For example, asking people what they think about a set of new product features
is a highly invasive measure that can yield inaccurate results. By contrast,
inconspicuously observing the way people interact with the features is a minimally
invasive measure, and will yield more reliable results.
In cases where highly invasive measures are used over long periods of time, it
is common for systems to become permanently altered in order to adapt to the
disruption of the measure. For example, the goal of standardized testing is to
measure student knowledge and predict achievement. However, the high stakes
associated with these tests change the system being measured: high stress levels
cause many students to perform poorly; schools focus on teaching the test to give
their students an advantage; students seek training on how to become test wise
and answer questions correctly without really knowing the answers; and so on. The
validity of the testing is thus compromised, and the invasiveness of the measure
fundamentally changes the focus of the system from learning to test-preparation.
Use low-invasive measures whenever possible. Avoid high-invasive measures;
they yield questionable results, reduce system efficiency, and can result in the
system adapting to the measures. Consider using natural system indicators of
performance when possible (e.g., number of widgets produced), rather than
measures that will consume resources and introduce interference (e.g., employee
log of hours worked).
See also Cost-Benefit, Expectation Effects, Feedback Loop, Framing, and
Signal-to-Noise Ratio.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

There is an inverse relationship
between the invasiveness and the
accuracy of system measures. The
more invasive the techniques to
measure a phenomenon, the less
accurate the measurements. In
extreme cases, invasive measures
can so severely disrupt a system
that it will alter its goal to serve the
measure, making measurement
meaningless. System efficiency also
suffers from invasive measurement
techniques, since system resources
must be applied increasingly to
accommodate the measurement.
Uncertainty Principle 245
System Behavior
System Efficiency
Invasiveness of Measure
Time

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Uncertainty Principle** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Uncertainty Principle để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Cost-Benefit, Expectation Effects, Feedback Loop, Framing, and
Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
