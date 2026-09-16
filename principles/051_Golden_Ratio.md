---
name: "Golden Ratio"
vi: "Tỷ lệ vàng (Golden Ratio)"
summary: "Golden Ratio (Tỷ lệ vàng (Golden Ratio)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Golden Ratio (Tỷ lệ vàng (Golden Ratio))

> **Tóm tắt cốt lõi (Summary)**: Golden Ratio là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

a 	b 	c

Golden Ratio
A ratio within the elements of a form, such as height to
width, approximating 0.618.1
The golden ratio is the ratio between two segments such that the smaller (bc)
segment is to the larger segment (ab) as the larger segment (ab) is to the sum of
the two segments (ac), or bc/ab = ab/ac = 0.618.2
The golden ratio is found throughout nature, art, and architecture. Pinecones,
seashells, and the human body all exhibit the golden ratio. Piet Mondrian and
Leonardo da Vinci commonly incorporated the golden ratio into their paintings.
Stradivari utilized the golden ratio in the construction of his violins. The Parthenon,
the Great Pyramid of Giza, Stonehenge, and the Chartres Cathedral all exhibit the
golden ratio.
While many manifestations of the golden ratio in early art and architecture were
likely caused by processes not involving knowledge of the golden ratio, it may
be that these manifestations result from a more fundamental, subconscious
preference for the aesthetic resulting from the ratio. A substantial body of
research comparing individual preferences for rectangles of various proportions
supports a preference based on the golden ratio. However, these findings have
been challenged on the theory that preferences for the ratio in past experiments
resulted from experimenter bias, methodological flaws, or other external factors.3
Whether the golden ratio taps into some inherent aesthetic preference or is
simply an early design technique turned tradition, there is no question as to its
past and continued influence on design. Consider the golden ratio when it is not
at the expense of other design objectives. Geometries of a design should not be
contrived to create golden ratios, but golden ratios should be explored when other
aspects of the design are not compromised.4
See also Aesthetic-Usability Effect, Form Follows Function, Rule of Thirds, and
Waist-to-Hip Ratio.
1 Also known as golden mean, golden number,
golden section, golden proportion, divine
proportion, and sectio aurea.
2 The golden ratio is irrational (never-ending
decimal) and can be computed with the
equation (ࠨ5-1)/2. Adding 1 to the golden
ratio yields 1.618…, referred to as Phi (o).
The values are used interchangeably to
define the golden ratio, as they represent the
same basic geometric relationship. Geometric
shapes derived from the golden ratio include
golden ellipses, golden rectangles, and
golden triangles.
3 The seminal work on the golden ratio is
Über die Frage des Golden Schnitts [On the
question of the golden section] by Gustav T.
Fechner, Archiv für die zeichnenden Künste
[Archive for the Drawn/Graphic Arts], 1865,
vol. 11, p. 100–112. A contemporary reference
is “All That Glitters: A Review of Psychological
Research on the Aesthetics of the Golden
Section” by Christopher D. Green, Perception,
1995, vol. 24, p. 937–968. For a critical
examination of the golden ratio thesis, see
“The Cult of the Golden Ratio” in Weird Water
& Fuzzy Logic by Martin Gardner, Prometheus
Books, 1996, p. 90–96.
4 The page spread of this book approximates a
golden rectangle. The page height is 10 inches
(25 cm) and the page width is 8.5 inches (22
cm). The total page-spread width (17 inches
[43 cm]) divided by the page height yields a
ratio of 1.7.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

In each example, the ratio between the
blue and red segments approximates
the golden ratio. Note how the ratio
corresponds with a significant feature
or alteration of the form.
Examples are the Parthenon,
Stradivarius Violin, Notre-Dame
Cathedral, Nautilus Shell, Eames
LCW Chair, Apple iPod MP3 Player,
and da Vinci’s Vitruvian Man.
Golden Ratio 115
A 	B
Golden Ratio
A/B = 1.618
B/A = 0.618
Golden Section

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Golden Ratio** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Golden Ratio để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Aesthetic-Usability Effect, Form Follows Function, Rule of Thirds, and
Waist-to-Hip Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
