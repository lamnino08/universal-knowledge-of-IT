---
name: "Archetypes"
vi: "Hình mẫu nguyên bản"
summary: "Archetypes (Hình mẫu nguyên bản): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Archetypes (Hình mẫu nguyên bản)

> **Tóm tắt cốt lõi (Summary)**: Archetypes là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Archetypes
Universal patterns of theme and form resulting from innate
biases or dispositions.
Archetypes are found in the themes of myths (e.g., death and rebirth), characters
in literature (e.g., hero and villain), and imagery in dreams (e.g., eyes and teeth).
They are believed to be a product of unconscious biases and dispositions that
have been “hardwired” in the brain over the course of human evolution. Since
these innate biases and dispositions are unconscious, their existence is inferred
when common patterns emerge in many cultures over long periods. Identifying
and aligning appropriate archetypes with a design will increase its probability of
success.1
Harley-Davidson aligns its product design and branding with the outlaw archetype,
emphasizing freedom and living outside the rules of society. Products have a
certain look and feel (e.g., black and chrome motorcycles with a loud, distinctive
sound) and marketing images emphasize rugged looking people in black leather.
Nike (named after the Greek goddess of victory), by contrast, aligns its brand with
the Hero archetype, using heroic sports figures to promote its product. Michael
Jordan, Tiger Woods, and Lance Armstrong are all shown wearing Nike products
while typically striking a heroic pose. This does not mean that a picture of Michael
Jordan on a Harley wouldn’t help sell motorcycles, or that a picture of a group of
outlaws wearing Nike leather jackets wouldn’t help sell sportswear. It does mean
that the probability of success would be lower because the archetypes do not align
with the design.2
In storytelling, archetypal themes are all too familiar. For example, one archetypal
plot—the Hero’s Journey—can be summarized as follows: a prospective hero is
called to an adventure that he or she refuses; a meeting with a mentor occurs and
the hero meets the call; the hero experiences various trials, often including the
defeat or death of the mentor by an ultimate enemy; the hero must overcome self-
doubt and confront the ultimate enemy; the hero defeats the ultimate enemy and
returns home to great celebration. This archetypal theme has been successfully
employed by filmmakers like George Lucas and George Miller, and is also evident
in the works of Steven Spielberg, John Boorman, Francis Coppola, and a number
of Disney animated films.3
Consider archetypal themes and forms in all aspects of a design—from form
and function to name and brand. Since archetypes influence perception on
an unconscious and primarily affective level, they are especially useful when
traditional modes of communication (e.g., language) cannot be used. Note that
reactions to specific archetypes may vary across cultures and, therefore, should
be tested on target populations prior to use.
See also Affordance, Biophilia Effect, Contour Bias, Mimicry, and
Threat Detection.

1 The seminal work on archetypes is “The
Archetypes and the Collective Unconscious”
by Carl G. Jung, in the Collected Works of C.
G. Jung, Vol. 9 Part 1 (translated by R. F. C.
Hull), Princeton University Press, 1981.
2 See The Hero and the Outlaw: Building
Extraordinary Brands through the Power of
Archetypes by Margaret Mark and Carol S.
Pearson, McGraw-Hill Trade, 2001.
3 The seminal work on archetypes in storytelling
is The Hero with a Thousand Faces by Joseph
Campbell, Princeton University Press, 1960.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

These are proposed designs for
a marker system to warn future
generations of the presence of a
nuclear- waste disposal site. The
design specification required the
markers to stand for the life of
the radioactive hazard (10,000
years), clearly warn people to stay
away from the area, and assume
that future civilizations will not be
knowledgeable of radioactive hazards
or speak any language known today.
The designs address this seemingly
impossible specification through the
brilliant application of archetypal
theme and form—parched earth,
snakelike earthworks, and claws and
thorns—to warn future humans of the
radioactive hazards on an affective,
instinctive level.
Archetypes 29

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Archetypes** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Archetypes để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Biophilia Effect, Contour Bias, Mimicry, and
Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
