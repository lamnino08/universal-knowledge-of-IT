---
name: "Scarcity"
vi: "Hiệu ứng khan hiếm (Scarcity)"
summary: "Scarcity (Hiệu ứng khan hiếm (Scarcity)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Scarcity (Hiệu ứng khan hiếm (Scarcity))

> **Tóm tắt cốt lõi (Summary)**: Scarcity là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Scarcity
Items and opportunities become more desirable when they
are perceived to be in short supply or occur infrequently.
Few principles move humans to action more effectively than scarcity. When items
and opportunities become scarce, their general desirability increases, and even
people who are otherwise disinterested often find themselves motivated to act.
The cause likely regards scarcity acting as an indicator of quality in combination
with a strong preference for keeping options open whenever possible — in other
words, when supply is scarce, demand appears high and the option to participate
is at risk. The principle applies generally across the spectrum of human behavior,
from mate attractiveness and selection (often referred to as the Romeo and Juliet
Effect) to tactics of negotiation.1
Five tactics are commonly employed to apply the principle:
Exclusive Information —	1. 	Supply is about to be depleted and only a few people
have this knowledge (e.g., don’t tell anyone, but a sugar shortage is about to
dramatically reduce the supply of cookies).
Limited Access —	2. 	Access to supply is limited (e.g., cookies available to first
class passengers only are more desirable than cookies available to all).
Limited Time —	3. 	Supply is available for a limited time (e.g., cookies available
one day a week are more desirable than cookies available every day).
Limited Number —	4. 	Supply is limited by number (e.g., a plate with two cookies
is more desirable than a plate with ten cookies).
Suddenness —	5. 	Supply is suddenly depleted (e.g., eight of ten cookies are
suddenly sold, making the remaining two cookies highly desirable).
When competition for scarce resources is visible and direct, the effects can be
contagious. This dynamic is commonly observed at auctions, where competing
bidders become fixated on winning and consequently bid well over market value
for an item. The effect is strongest when the desired object or opportunity is highly
unique, and not easily obtained or approximated by other means.2
Consider scarcity when designing advertising and promotion initiatives, especially
when the objective is to move people to action. Scarce items are accorded higher
value than plentiful items, so ensure that pricing and availability are aligned. In
retail contexts, do not confuse having inventory with the need to display
inventory — displays that show a lot of product will sell less quickly than retail
displays that show small amounts. Make the effects of demand, especially sudden
demand, clearly visible whenever possible to achieve maximum effect.
See also Expectation Effect, Framing, and Veblen Effect.
1 The seminal works on scarcity are A Theory
of Psychological Reactance by Jack Brehm,
Academic Press, 1966; and “Implications
of Commodity Theory for Value Change”
by Timothy Brock, in A.G. Greenwald, T.C.
Brock, and T.M. Ostrom (Eds.), Psychological
Foundations of Attitudes, Academic Press,
1968. For a popular treatment of the principle,
see Influence: The Psychology of Persuasion
by Robert Cialdini, Collins Business, 2006.
2 “Scarcity Effects on Value: A Quantitative
Review of the Commodity Theory Literature” by
Michael Lynn, Psychology & Marketing, Spring
1991, vol. 8(1), p. 43–57.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

In a classic illustration of the power of
scarcity, the “Running of the Brides”
event at Filene’s Basement has
brides-to-be coming from around
the world to buy wedding dresses
at bargain basement prices. The
event is held once a year, one day
only. Friends and family help box out
competitors and snatch up dresses
as quickly as possible. Brides try
candidate dresses on in the aisles
until they find that special dress.
All of the factors of scarcity are at
play: exclusive information, limited
access, limited time, limited number,
suddenness, and visibility of demand.
Scarcity 217

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Scarcity** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Scarcity để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Expectation Effect, Framing, and Veblen Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
