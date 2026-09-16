---
name: "Color"
vi: "Lý thuyết màu sắc"
summary: "Color (Lý thuyết màu sắc): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - appeal
---

# Universal Design Principle: Color (Lý thuyết màu sắc)

> **Tóm tắt cốt lõi (Summary)**: Color là một nguyên lý thiết kế then chốt thuộc nhóm **perception, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Color is used in design to attract attention, group
elements, indicate meaning, and enhance aesthetics.
Color can make designs more visually interesting and aesthetic, and can reinforce
the organization and meaning of elements in a design. If applied improperly,
however, color can seriously harm the form and function of a design. The following
guidelines address common issues regarding the use of color.1
Number of Colors
Use color conservatively. Limit the palette to what the eye can process at one
glance (about five colors depending on the complexity of the design). Do not use
color as the only means to impart information since a significant portion of the
population has limited color vision.
Color Combinations
Achieve aesthetic color combinations by using adjacent colors on the color wheel
(analogous), opposing colors on the color wheel (complementary), colors at
the corners of a symmetrical polygon circumscribed in the color wheel (triadic
and quadratic), or color combinations found in nature. Use warmer colors for
foreground elements, and cooler colors for background elements. Light gray is a
safe color to use for grouping elements without competing with other colors.
Saturation
Use saturated colors (pure hues) when attracting attention is the priority. Use
desaturated colors when performance and efficiency are the priority. Generally,
desaturated, bright colors are perceived as friendly and professional; desaturated,
dark colors are perceived as serious and professional; and saturated colors are
perceived as more exciting and dynamic. Exercise caution when combining
saturated colors, as they can visually interfere with one another and increase
eye fatigue.
Symbolism
There is no substantive evidence supporting general effects of color on emotion
or mood. Similarly, there is no universal symbolism for different colors—different
cultures attach different meanings to colors. Therefore, verify the meaning of
colors and color combinations for a particular target audience prior to use.2
See also Expectation Effect, Highlighting, Interference Effects, Similarity, and
Uniform Connectedness.

1 A nice treatment of color theory is Interaction
of Color by Josef Albers, Yale University Press,
1963. For a more applied treatment, see The
Art of Color: The Subjective Experience and
Objective Rationale of Color by Johannes
Itten, John Wiley & Sons, 1997; and Human-
Computer Interaction by Jenny Preece, et al.,
Addison Wesley, 1994.
2 It is reasonable to assume that dark colors will
make people sleepy, light colors will make
people lively, and irritating colors will make
people irritated. Otherwise, the only observable
influence of color on behavior is its ability to
lead people to repaint walls unnecessarily. For
those determined to try to calm drunks and
win football games through the application
of color, see The Power of Color by Morton
Walker, Avery Publishing, 1991.
Color

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Analogous color combinations use
colors that are next to each other on
the color wheel.
Complementary color combinations
use two colors that are directly across
from each other on the color wheel.
Hues from yellow to red-violet on the
color wheel are warm. Hues from
violet to green-yellow are cool.
Saturation refers to the amount of
gray added to a hue. As saturation
increases, the amount of gray
decreases. Brightness refers to the
amount of white added to a hue—as
brightness increases, the amount of
white increases.
Triadic color combinations use colors
at the corners of an equilateral triangle
circumscribed in the color wheel.
Quadratic color combinations use
colors at that corners of a square
or rectangle circumscribed in the
color wheel.
Color 49
warm
cool
Analogous 	Example from Nature 	Triadic 	Example from Nature
Complementary 	Example from Nature 	Quadratic 	Example from Nature
Saturation
Brightness

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Color** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Color để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Expectation Effect, Highlighting, Interference Effects, Similarity, and
Uniform Connectedness
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
