---
name: "Priming"
vi: "Mồi nhận thức (Priming)"
summary: "Priming (Mồi nhận thức (Priming)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Priming (Mồi nhận thức (Priming))

> **Tóm tắt cốt lõi (Summary)**: Priming là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Priming
The activation of specific concepts in memory for the
purposes of influencing subsequent behaviors.
Whenever stimuli are received by the senses — sights, sounds, smells, touches,
tastes — concepts are automatically activated in memory. Once concepts
are activated, they stay activated for a period of time, capable of influencing
subsequent thoughts, reactions, emotions, and behaviors. For example, in a
classic experiment on the effects of priming, two groups of college students were
given a series of written language tests. The language test for one group included
words related to politeness, and the language test for the other group included
words related to rudeness. Subjects were instructed to complete the test, and
then go down the hall and find the test administrator to get instructions for their
next task. When each student completed his or her test and went down the hall,
the student found the test administrator engaged in a conversation with another
person. Unbeknownst to the students, the real test regarded whether the students
would interrupt the conversation, or wait politely until the conversation ended.
The results were dramatic: 63 percent of the students primed with words related
to rudeness interrupted, whereas only 17 percent primed with words related to
politeness interrupted. Exposure to words related to politeness made people more
polite, and exposure to words to related to rudeness made people ruder.1
Priming is an effective means of influence when the stimulus introduced activates
concepts that are consistent with a preexisting need or goal. For example, showing
an image of a person drinking soda before a movie would have an effect on thirsty
people, inducing more of them to buy soda than would otherwise, but it would
have no effect on nonthirsty people. However, since everyone in the audience
shares the goal of wanting to see a good movie, showing positive imagery and
movie previews will prime the audience to react more favorably to the movie
generally than they would otherwise. It is this latter kind of indirect prime — the
prime that is unnoticed — that is the most effective. When viewing a typical
advertisement, the audience knows there is an attempt at influence, and they
may consciously counteract it. By contrast, when the students in the experiment
were primed for rudeness or politeness, there was no obvious direct link and no
conscious awareness of the manipulation. If you told them why they were being so
rude or so polite, they would respond with incredulity.
Consider priming in all aspects of design. First impressions, contexts, and
antecedent events are all opportunities to influence subsequent reactions and
behaviors — this includes the way products are presented in packaging, the
articles adjacent to advertisements in newspapers, and the experiences leading
from the parking lot to the entryway of a retail store. Favor indirect primes over
direct primes, as the former tends to be more persistent and leaves no trace.
See also Cathedral Effect, Expectation Effect, and Exposure Effect.
1 The seminal work on priming as it pertains to
influence is “Automaticity of Social Behavior:
Direct Effects of Trait Construct and Stereotype
Activation on Action” by John Bargh, Mark
Chen, and Lara Burrows, Journal of Personality
and Social Psychology, 1996, vol. 71(2), p.
230–244. See also “Losing Consciousness:
Automatic Influences on Consumer Judgment,
Behavior, and Motivation” by John Bargh, The
Journal of Consumer Research, Sept. 2002,
vol. 29(2), p. 280–285.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Priming 187
Psychologists at Newcastle University
observed that staff members using
an honor system coffee station often
did not contribute money when they
drank the coffee. As psychologists are
inclined to do, they decided to run
an experiment. For ten weeks they
alternately taped two posters over
the coffee station. The first poster
featured a generic image, and the
second poster featured staring eyes.
The results were striking: When the
poster with the eyes was displayed
people contributed almost three times
more money than they did when the
poster with the generic image was
displayed. Whether people consciously
noticed the poster or not, the eyes
in the poster activated regions of the
brain that regarded being watched,
increasing the sense of accountability
and, by extension, the coffee fund.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Priming** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Priming để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Cathedral Effect, Expectation Effect, and Exposure Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
