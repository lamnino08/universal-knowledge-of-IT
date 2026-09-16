---
name: "Stickiness"
vi: "Tính ghi nhớ bền lâu (Stickiness)"
summary: "Stickiness (Tính ghi nhớ bền lâu (Stickiness)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - appeal
---

# Universal Design Principle: Stickiness (Tính ghi nhớ bền lâu (Stickiness))

> **Tóm tắt cốt lõi (Summary)**: Stickiness là một nguyên lý thiết kế then chốt thuộc nhóm **learning, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Stickiness
A method for dramatically increasing the recognition,
recall, and unsolicited sharing of an idea or expression.
Popularized by Malcolm Gladwell in his book The Tipping Point, the term
stickiness refers to the ability of certain ideas to become lodged in the cul-
tural consciousness. Stickiness applies to anything that can be seen, heard, or
touched — slogans, advertisements, and products. Six variables appear to be key
in the creation of sticky ideas:1
Simplicity —	1. 	The idea can be expressed simply and succinctly, without
sacrificing depth (e.g., “It’s the economy, stupid,” used during Bill Clinton’s
1992 U.S. presidential campaign).
Surprise —	2. 	The idea contains an element of surprise, which grabs attention
(e.g., when the Center for Science in the Public Interest wanted to alarm
consumers to the amount of fat in movie popcorn, they noted that it had
more fat than “a bacon-and-eggs breakfast, a Big Mac and fries for lunch,
and a steak dinner with all the trimmings — combined!”).
Concreteness —	3. 	The idea is specific and concrete, using plain language or
imagery (e.g., John F. Kennedy’s 1962 moon speech: “We choose to go to
the moon in this decade…”).
Credibility —	4. 	The idea is believable, often communicated by a trusted source
or as an appeal to common sense (e.g., Subway restaurants’ Jared campaign
engaged the personal testimonials of Jared Fogle, complete with before and
after photographs, to show the benefits of his Subway sandwich diet).
Emotion —	5. 	The idea elicits an emotional reaction (e.g., on Halloween in
the 1960s and 1970s, false rumors circulated that sadists were putting
razor blades in apples, panicking parents and effectively shutting down the
tradition of trick-or-treating for much of the United States).
Story —	6. 	The idea is expressed in the context of a story, dramatically
increasing its memorability and retelling (e.g., the Cabbage Patch Kids craze
was due to the story attached to them — each doll is uniquely featured,
named, and delivered with a birth certificate from BabyLand Hospital).
Consider stickiness in the design of instruction, advertising, products, and other
contexts involving memory. Keep messaging succinct, but profound. Employ sur-
prise to capture attention and motivate sharing. Ensure that ideas are expressed
using specific time frames and objects or events that are available to the senses.
Favor presenting evidence and letting people draw their own conclusions.
Incorporate affective triggers to evoke a strong emotional response. Couch ideas in
rich contexts to improve memorability and transmissibility.
See also Archetypes, Propositional Density, Storytelling, and von Restorff Effect.
1 The seminal work on stickiness is Made to
Stick: Why Some Ideas Survive and Others
Die by Chip Heath and Dan Heath, Random
House, 2007.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Stickiness 229
This iconic poster by artist Shepard
Fairey became synonymous with the
2008 Obama presidential campaign.
The poster’s simple message, unique
aesthetic, and emotional grass-roots
appeal made it incredibly sticky,
creating a viral sharing phenomenon
as soon as Fairey posted the image
on the Web.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Stickiness** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Stickiness để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Archetypes, Propositional Density, Storytelling, and von Restorff Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
