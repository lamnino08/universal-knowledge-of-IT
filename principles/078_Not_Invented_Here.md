---
name: "Not Invented Here"
vi: "Hội chứng không phát minh tại đây (NIH)"
summary: "Not Invented Here (Hội chứng không phát minh tại đây (NIH)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Not Invented Here (Hội chứng không phát minh tại đây (NIH))

> **Tóm tắt cốt lõi (Summary)**: Not Invented Here là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Not Invented Here
A bias against ideas and innovations that
originate elsewhere.
The not invented here (NIH) syndrome is an organizational phenomenon in which
groups resist ideas and inputs from external sources, often resulting in subpar
performance and redundant effort (i.e., “reinventing the wheel”). Examples
abound. When Phillips bought Sonicare, manufacturer of the very popular
Sonicare toothbrush, Phillips decided to redesign and reengineer the product,
though there was no compelling need to do so. A similar questionable redesign
occurred with the American introduction of the Sinclair Spectrum computer, which
Timex reengineered and released as the Timex 2068. The changes increased
the computer’s capability, but the cost was a bland form factor and numerous
software incompatibilities, resulting in a failed product. Long after market feedback
and usability research indicated that the optimum number of buttons for a
computer mouse was two, Apple stubbornly refused to change and maintained
its one-button mouse design. When a devoted owner of an AIBO created an
application that enabled the robot dog to dance to music, Sony responded with
a lawsuit threat to quash the effort. What drives organizations to engage in these
kinds of counterproductive NIH behaviors?
Four social dynamics underlie NIH: belief that internal capabilities are superior
to external capabilities; fear of losing control; desire for credit and status; and
significant emotional and financial investment in internal initiatives. NIH resulting
from a perception of superiority is often pervasive in organizations with a proud
legacy of successful innovation; their past successes effectively sabotage their
capacity to consider external sources. Correction typically requires a significant
failure to humble the organization and reset the culture. Fear of losing control is
common when groups perceive a risk to their jobs or status in an organization,
but it is also common when products are used in unexpected ways. Correction
typically requires clear goals and direction from management with clarification
regarding how staff members fit into the operating plan. NIH resulting from
investments in current or legacy initiatives is difficult to overcome. Correction
typically requires significant organizational change or a change in leadership.2
The best way to address NIH is prevention. Rotate and cross-pollinate team
members on a project basis. Engage outsiders in both the strategy and the
evaluation stages of the design process to ensure fresh perspectives and new
thinking. Encourage team members to regularly interact with the wider community
(e.g., conferences). Formalize regular competitor reviews and environmental
scanning to stay abreast of the activities of competitors and the industry in
general. Consider open innovation models, competitions (e.g., Netflix Prize), and
outside collaborations to institutionalize a meritocratic approach to new ideas.
Lastly, teach team members about the causes, costs, and remedies for NIH, as
recognition is the first step to prevention and recovery.3
See also Cognitive Dissonance, Design by Committee, Life Cycle, and Mimicry.
1 The seminal works on NIH are “Receptivity
to Innovation — Overcoming NIH” by Robert
Clagett, Master’s Thesis, MIT, 1967; and
“Investigating the Not-Invented-Here (NIH)
Syndrome: A Look at Performance, Tenure
and Communication Patterns of 50 R&D
Project Groups” by Ralph Katz and Thomas
Allen, R&D Management, 1982, vol. 12, p.
7–19.
2 See, for example, Strategies for Supplier
Integration by Robert M. Monczka, Robert
B. Handfield, Thomas V. Scannell, et al.,
American Society for Quality, 2000, p.
178–179; and Management of Research and
Development Organizations by Ravinder Jain
and Harry Triandis, Wiley, 1997, p. 36–38.
3 See, for example, Open Business Models:
How to Thrive in the New Innovation
Chesbrough, Harvard Business School Press,
2006.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Not Invented Here 169
In 1982, the Sinclair ZX81 was
licensed to Timex for resale in the
United States as the Timex Sinclair
1000. The computers were identical
except for the name on the case and
minor motherboard differences. Sales
were strong. With subsequent models,
however, NIH syndrome inclined
Timex to introduce more and more
changes. Eventually, the product
divergence created issues of software
compatibility — costs went up, sales
went down. Timex dropped out of the
computer market in 1984.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Not Invented Here** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Not Invented Here để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Cognitive Dissonance, Design by Committee, Life Cycle, and Mimicry
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
