---
name: "Constancy"
vi: "Hằng định nhận thức (Constancy)"
summary: "Constancy (Hằng định nhận thức (Constancy)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Constancy (Hằng định nhận thức (Constancy))

> **Tóm tắt cốt lõi (Summary)**: Constancy là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The tendency to perceive objects as unchanging, despite
changes in sensory input.1
People tend to perceive objects as constant and unchanging, despite changes in
perspective, lighting, color, or size. For example, a person viewed at a distance
produces a smaller image on the retina than that same person up close, but the
perception of the size of the person is constant. The ability to perceive objects as
having constant properties despite variations in how they are perceived eliminates
the need to reinterpret those objects when they are perceived under different
conditions. This indicates that perception involves more than simply receiving
sensory inputs; rather, it is a process of continuously reconciling sensory inputs
with memories about the properties of things in the world. A few examples of
constancy include: 2
Size Constancy —The size of objects is perceived to be constant, even though
a change in distance makes objects appear smaller or larger (e.g., a city skyline
at a great distance appears small, but the perception of the size of the buildings
remains constant).
Brightness Constancy —The brightness of objects is perceived to be constant,
even though changes in illumination make the objects appear brighter or darker
(e.g., a white shirt appears gray in a dark room, but the perception of the color of
the shirt remains constant).
Shape Constancy —The shape of objects is perceived to be constant, even though
changes in perspective make the objects appear to have different shapes (e.g., a
wheel from the side appears circular, at an angle it appears elliptical, and from the
front it appears rectangular, but the perception of the shape of the wheel remains
constant).
Loudness Constancy —The loudness of a sound is perceived to be constant, even
though a change in distance makes the sound seem softer or louder (e.g., music
playing on a radio seems to get softer as you walk away from it, but the perception
of the volume of the radio remains constant).
All senses exhibit constancy to some extent. Consider the tendency when
designing high-fidelity renderings, simulations, or models of objects and
environments. For example, changes in properties like distance, perspective,
and illumination should change appropriately for the type of interaction. Use
recognizable objects and distance cues to provide size and shape references
for unfamiliar objects. Consider illumination levels and background colors in
environments when making decisions about color and brightness levels; lighting
and color variations in the environment can trick the senses and alter the
perception of color.
See also Color, Highlighting, Interference Effects, and Orientation Sensitivity.

1 Also known as perceptual constancy.
2 Seminal works on constancy include
“Brightness Constancy and the Nature of
Achromatic Colors” by Hans Wallach, Journal
of Experimental Psychology, 1948, vol. 38,
p. 310–324; and “Determinants of Apparent
Visual Size With Distance Variant” by A.
F. Holway and Edwin G. Boring, American
Journal of Psychology, 1941, vol. 54, p. 21–37.
A nice review of the various forms of constancy
is found in Sensation and Perception by
Margaret W. Matlin and Hugh J. Foley, 4th
ed., Allyn & Bacon, 1997.
Constancy

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Despite their apparent differences, the
pair of circles within the grid blocks
are the same color and brightness—
a fact easily revealed by covering the
areas surrounding the circles.
The perceived differences are caused
by correction errors made by the
visual processing system, which tries
to maintain constancy by offsetting
color and brightness variations across
different background conditions.
Constancy 59

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Constancy** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Constancy để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Color, Highlighting, Interference Effects, and Orientation Sensitivity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
