---
name: "Expectation Effect"
vi: "Hiệu ứng kỳ vọng"
summary: "Expectation Effect (Hiệu ứng kỳ vọng): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Expectation Effect (Hiệu ứng kỳ vọng)

> **Tóm tắt cốt lõi (Summary)**: Expectation Effect là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A phenomenon in which perception and behavior changes
as a result of personal expectations or the expectations
of others.
The expectation effect refers to ways in which expectations affect perception and
behavior. Generally, when people are aware of a probable or desired outcome,
their perceptions and behavior are affected in some way. A few examples of this
phenomenon include:1
Halo Effect—Employers rate the performance of certain employees more
highly than others based on their overall positive impression of those
employees.
Hawthorne Effect—Employees are more productive based on their belief that
changes made to the environment will increase productivity.
Pygmalion Effect—Students perform better or worse based on the
expectations of their teacher.
Placebo Effect—Patients experience treatment effects based on their belief
that a treatment will work.
Rosenthal Effect—Teachers treat students differently based on their
expectations of how students will perform.
Demand Characteristics—Participants in an experiment or interview provide
responses and act in ways that they believe are expected by the experimenter
or interviewer.
The expectation effect demonstrates that expectations can greatly influence
perceptions and behavior. For example, tell a large group of people that a new
product will change their lives, and a significant number will find their lives
changed—the belief is simply a device that helps create the change. Once a
person believes something will happen, the belief alone creates that possibility.
Unfortunately, this can have a negative impact on the ability to accurately measure
a design’s success. Since designers are naturally biased toward their designs,
they often unintentionally influence test subjects through words or actions, or may
omit certain results in order to corroborate their expectations. Test subjects often
respond by seeking to meet the expectations communicated to them.
Consider the expectation effect when introducing and promoting a design.
When trying to persuade, set expectations in a credible fashion for the target
audience rather than letting them form their own unbiased conclusions. When
evaluating a design, use proper test procedures to avoid biases resulting from
the expectation effect.
See also Exposure Effect, Framing, and Uncertainty Principle.
1 Seminal works on the expectation effect
include The Human Problems of an Industrial
Civilization by Elton Mayo, Macmillan, 1933;
“The Effect of Experimenter Bias on the
Performance of the Albino Rat” by Robert
Rosenthal and Kermit Fode, Behavioral
Science, 1963, vol. 8, p. 115–118; “Teachers’
Expectancies: Determinants of Pupils’ IQ
Gains” by Robert Rosenthal and Lenore
Jacobson, Psychological Reports, vol.
19, p. 115–118. For a nice review of the
placebo effect, see The Placebo Effect: An
Interdisciplinary Exploration edited by Anne
Harrington, Harvard University Press, 1999.
Expectation Effect

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The expectation effect can influence
perception and behavior, but
the changes are temporary. For
example, the marker along the time
axis indicates the point at which an
expectation was set. A change in
performance may be observed as a
result (e.g., increased productivity) but
usually reverts back to baseline.
A credible presentation will generate an
expectation effect in about 30 percent
of any given audience. Keeping the
claims and outcomes vague often
helps—a believing person is biased
to interpret ambiguous effects in
accordance with their expectations.
This technique was used to sell snake
oil solutions, and is still widely used to
sell astrology, psychic predictions, and
things such as fad diets.
Expectation Effect 85
SAGITTARIUS
November 23–December 21
It’s a favorable time for real estate, investments, and
moneymaking opportunities to be successful. Romance
could develop through social activities or short trips. Don’t
expect new acquaintances to be completely honest about
themselves. Your lucky day this week will be Sunday.
Time
Performance

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Expectation Effect** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Expectation Effect để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Exposure Effect, Framing, and Uncertainty Principle
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
