---
name: "Interference Effects"
vi: "Hiệu ứng nhiễu giao thoa (Interference Effects)"
summary: "Interference Effects (Hiệu ứng nhiễu giao thoa (Interference Effects)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - learning
  - usability
---

# Universal Design Principle: Interference Effects (Hiệu ứng nhiễu giao thoa (Interference Effects))

> **Tóm tắt cốt lõi (Summary)**: Interference Effects là một nguyên lý thiết kế then chốt thuộc nhóm **perception, learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Interference Effects
A phenomenon in which mental processing is made slower
and less accurate by competing mental processes.
Interference effects occur when two or more perceptual or cognitive processes are
in conflict. Human perception and cognition involve many different mental systems
that parse and process information independently of one another. The outputs of
these systems are communicated to working memory, where they are interpreted.
When the outputs are congruent, the process of interpretation occurs quickly and
performance is optimal. When outputs are incongruent, interference occurs and
additional processing is needed to resolve the conflict. The additional time required
to resolve such conflicts has a negative impact on performance. A few examples of
interference effects include: 1
Stroop Interference—an irrelevant aspect of a stimulus triggers a mental process
that interferes with processes involving a relevant aspect of the stimulus. For
example, the time it takes to name the color of words is greater when the meaning
and color of the words conflict.
Garner Interference—an irrelevant variation of a stimulus triggers a mental
process that interferes with processes involving a relevant aspect of the stimulus.
For example, the time it takes to name shapes is greater when they are presented
next to shapes that change with each presentation.
Proactive Interference—existing memories interfere with learning. For example,
in learning a new language, errors are often made when people try to apply the
grammar of their native language to the new language.
Retroactive Interference—learning interferes with existing memories. For
example, learning a new phone number can interfere with phone numbers
already in memory.
Prevent interference by avoiding designs that create conflicting mental processes.
Interference effects of perception (i.e., Stroop and Garner) generally result from
conflicting coding combinations (e.g., a red go button, or green stop button) or
from an interaction between closely positioned elements that visually interact with
one another (e.g., two icons group or blend because of their shape and proximity).
Minimize interference effects of learning (i.e., proactive and retroactive) by mixing
the presentation modes of instruction (e.g., lecture, video, computer, activities),
employing advance organizers, and incorporating periods of rest every thirty to
forty-five minutes.
See also Advance Organizer, Performance Load, Errors, and Mapping.

1 The seminal works on interference effects
include “Studies of Interference in Serial
Verbal Reactions” by James R. Stroop,
Journal of Experimental Psychology, 1935,
vol. 28, p. 643–662; “Stimulus Configuration
in Selective Attention Tasks” by James R.
Pomerantz and Wendell R. Garner, Perception
& Psychophysics, 1973, vol. 14, p. 565–569;
and “Characteristics of Word Encoding” by
Delos D. Wickens, in Coding Processes in
Human Memory edited by A. W. Melton and
E. Martin, V. H. Winston, 1972, p. 191–215.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Red
Pink
Yellow
Black
Green
Purple
White
Orange
Gray
In populations that have learned
that green means go and red means
stop, the incongruence between the
color and the label-icon results
in interference.
In populations that have learned
that a traffic arrow always means go,
the introduction of a red arrow in
new traffic lights creates potentially
dangerous interference.
Reading the words aloud is easier
than naming their colors. The mental
process for reading is more practiced
and automatic and, therefore,
interferes with the mental process
for naming the colors.
Naming the column of shapes that
stands alone is easier than naming
either of the columns located together.
The close proximity of the columns
results in the activation of mental
processes for naming proximal
shapes, creating interference.
Interference Effects 139
STOP	GO
Trial 1 	Trial 2

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Interference Effects** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Interference Effects để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Advance Organizer, Performance Load, Errors, and Mapping
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
