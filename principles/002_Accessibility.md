---
name: "Accessibility"
vi: "Khả năng tiếp cận"
summary: "Accessibility (Khả năng tiếp cận): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - learning
  - decision
---

# Universal Design Principle: Accessibility (Khả năng tiếp cận)

> **Tóm tắt cốt lõi (Summary)**: Accessibility là một nguyên lý thiết kế then chốt thuộc nhóm **usability, learning, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Accessibility
Objects and environments should be designed to be usable,
without modification, by as many people as possible.1
The principle of accessibility asserts that designs should be usable by people of
diverse abilities, without special adaptation or modification. Historically, accessibility
in design focused on accommodating people with disabilities. As knowledge and
experience of accessible design increased, it became increasingly clear that many
required “accommodations” could be designed to benefit everyone. There are
four characteristics of accessible designs: perceptibility, operability, simplicity,
and forgiveness.2
Perceptibility is achieved when everyone can perceive the design, regardless
of sensory abilities. Basic guidelines for improving perceptibility are: present
information using redundant coding methods (e.g., textual, iconic, and tactile);
provide compatibility with assistive sensory technologies (e.g., ALT tags for images
on the Internet); and position controls and information so that seated and standing
users can perceive them.
Operability is achieved when everyone can use the design, regardless of physical
abilities. Basic guidelines for improving operability are: minimize repetitive actions
and the need for sustained physical effort; facilitate use of controls through
good affordances and constraints; provide compatibility with assistive physical
technologies (e.g., wheelchair access); and position controls and information so
that seated and standing users can access them.
Simplicity is achieved when everyone can easily understand and use the design,
regardless of experience, literacy, or concentration level. Basic guidelines for
improving simplicity are: remove unnecessary complexity; clearly and consistently
code and label controls and modes of operation; use progressive disclosure to
present only relevant information and controls; provide clear prompting and
feedback for all actions; and ensure that reading levels accommodate a wide
range of literacy.
Forgiveness is achieved when designs minimize the occurrence and consequences
of errors. Basic guidelines for improving forgiveness are: use good affordances and
constraints (e.g., controls that can only be used the correct way) to prevent errors
from occurring; use confirmations and warnings to reduce the occurrence of errors;
and include reversible actions and safety nets to minimize the consequence of
errors (e.g., the ability to undo an action).
See also Affordance, Forgiveness, Legibility, Normal Distribution, and Readability.
1 Also known as barrier-free design and related
to universal design and inclusive design.
2 The four characteristics of accessible
designs are derived from W3C Web Content
Accessibility Guidelines 1. 0, 1999; ADA
Accessibility Guidelines for Buildings and
Facilities, 1998; and Accessible Environments:
Toward Universal Design by Ronald L. Mace,
Graeme J. Hardie, and Jaine P. Place, The
Center for Universal Design, North Carolina
State University, 1996.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1 2 3 4 5 6
1 	2 	3 	4 	5 	6
1	2
3	4
5	6
EMERGENCY
	TELEPHONE
Accessibility 17
The large elevator has many features
that make it more accessible than
the small elevator: wide doors permit
easy access; handrails help people
maintain a standing position; two
sets of controls are easily accessible
from a seated position; controls are
redundantly coded with numbers,
icons, and Braille; feedback is
provided visually and aurally; and
an emergency phone system offers
access to special assistance.
Aural feedback
Visual feedback
Buttons with raised numbers and Braille
Emergency phone system
Doors wide enough for wheelchairs
Buttons on both sides of door
Buttons accessible from wheelchair
Elevator large enough for wheelchair
Handrails

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Accessibility** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Accessibility để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Forgiveness, Legibility, Normal Distribution, and Readability
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
