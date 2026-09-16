---
name: "Propositional Density"
vi: "Mật độ mệnh đề ý niệm (Propositional Density)"
summary: "Propositional Density (Mật độ mệnh đề ý niệm (Propositional Density)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Propositional Density (Mật độ mệnh đề ý niệm (Propositional Density))

> **Tóm tắt cốt lõi (Summary)**: Propositional Density là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Propositional Density
The relationship between the elements of a design and
the meaning they convey. Designs with high propositional
density are more interesting and memorable than designs
with low propositional density.
Propositional density is the amount of information conveyed in an object or
environment per unit element.1 High propositional density is a key factor in
making designs engaging and memorable — it is what makes double entendres
interesting and puns funny (i.e., they express multiple meanings with a single
phrase). For present purposes, a proposition is an elementary statement about
an object or environment that cannot be easily broken down into constituent
propositions. There are two types of propositions: surface propositions and deep
propositions. Surface propositions are the salient perceptible elements of an object
or environment. Deep propositions are the underlying and often hidden meanings
of those elements. Propositional density can be estimated by dividing the number
of deep propositions by the number of surface propositions, or mathematically:
PD 5 Pd / Ps
where:
PD is propositional density.
Pd is the number of deep propositions.
Ps is the number of surface propositions.
Objects and environments with high PD (PD > 1) are perceived to be more
interesting and engaging than objects and environments with low PD (PD < 1).
Simple objects and environments (i.e., few surface propositions) that are rich
in meaning (many deep propositions) are perceived to be the most compelling.
Consider, for example, the modern Apple, Inc., logo. The surface propositions
expressed by the logo are the body of the apple, top leaf, and missing chunk.
The deep propositions include, but are not limited to, the following: The apple
is a healthy fruit; the apple tree is the biblical tree of knowledge; a bite from the
apple represents a means to attain knowledge; Sir Isaac Newton’s epiphany about
gravity came from a falling apple; an apple a day keeps the doctor away; an apple
is an appropriate gift for a teacher; and so on. With just the propositions listed, the
Apple logo would have a PD 5 2, a high propositional density that makes the logo
interesting to look at and easy to remember.
Consider propositional density in all aspects of design. Favor simple elements that
are rich in meaning. Aspire to achieve the highest propositional density possible,
but make sure the deep propositions are complementary. Contradictory deep
propositions can confuse the message and nullify prospective benefits.
See also Archetypes, Cost-Benefit, Layering, and Signal-to-Noise Ratio.
1 The seminal theoretical work on propositional
density is Syntactic Structures by Noam
Chomsky, Mouton & Co., 1957. For other
examples of practical applications, see
“Building Great Sentences: Exploring the
Writer’s Craft” by Brooks Landon, The
Teaching Company, Course No. 2368, 2008;
“A Plain Man’s Guide to the Theory of Signs
in Architecture” by Geoffrey Broadbent, in
Theorizing a New Agenda for Architecture:
An Anthology of Architectural Theory by Kate
Nesbitt, Princeton Architectural Press, 1996,
p. 124–141.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The logo of Barack Obama’s 2008
presidential campaign has received
wide acclaim for its design, but the
logo’s high propositional density
(PD 5 10 / 3 5 3.33) is the prime
cause of its success.
The circle represents stability. 	The blue represents sky.
The sun rising represents change.
The logo contains a blue circle.
The logo contains red and white
lines.
The red and white lines cut
across the lower half of the circle.
The circle represents unity.
The circle represents an O for
Obama.
The red and white lines represent
amber waves of grain.
The red and white lines represent
a landscape.
The center of the circle
represents a sun rising.
The red and white lines represent
the American flag.
The red and white lines represent
patriotism.
Propositional Density 191

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Propositional Density** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Propositional Density để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Archetypes, Cost-Benefit, Layering, and Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
