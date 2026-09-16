---
name: "Three-Dimensional Projection"
vi: "Phép chiếu không gian ba chiều (3D Projection)"
summary: "Three-Dimensional Projection (Phép chiếu không gian ba chiều (3D Projection)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Three-Dimensional Projection (Phép chiếu không gian ba chiều (3D Projection))

> **Tóm tắt cốt lõi (Summary)**: Three-Dimensional Projection là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A tendency to see objects and patterns as three-
dimensional when certain visual cues are present.
People have evolved to see things as three-dimensional whenever possible—even
when the things are clearly not three-dimensional. The following visual cues are
commonly used to encourage the perception of three-dimensional relationships:1
Interposition
When two overlapping objects are presented, the overlapped object is perceived to
be farther away than the overlapping object.
Size
When two similar objects of different size are presented together, the smaller object
is perceived to be farther away than the larger object. The size of familiar objects
can also be used to indicate the size and depth of unfamiliar objects.
Elevation
When two objects are presented at different vertical locations, the object at the
higher elevation is perceived to be farther away.2
Linear Perspective
When two vertical lines converge near their top ends, the converging ends of the
lines are perceived to be farther away than the diverging ends.
Texture Gradient
When the texture of a surface varies in density, the areas of greater density are
perceived to be farther away than areas of lesser density.
Shading
When an object has shading or shadows, the shaded areas are perceived to be
the farthest away from the light source and the light areas are interpreted as being
closest to the light source.
Atmospheric Perspective
When multiple objects are presented together, the objects that are bluer and blurrier
are perceived to be farther away than the objects that are less blue and blurry.3
Consider these visual cues in the depiction of three-dimensional elements and
environments. Strongest depth effects are achieved when the visual cues are used
in combination; therefore, use as many of the cues as possible to achieve the
strongest effect, making sure that the cues are appropriate for the context.
See also Figure-Ground Relationship and Top-Down Lighting Bias.

1 Note that only static cues (as opposed to
motion cues) are presented here. A nice review
the various depth cues is found in Sensation
and Perception by Margaret W. Matlin and
Hugh J. Foley, Allyn & Bacon, 1997, p.
165–193.
2 An exception to this is when a strong
horizontal element is present, which tends to
be perceived as a horizon line. In this case,
objects that are closer to the horizon line are
perceived as farther away than objects that
are distant from the horizon line.
3 The relationship between the degree of
blueness and blurriness to distance is a
function of experience—i.e., people who live in
a smoggy city will have a different sense
of atmospheric perspective than people who live
in less-polluted rural areas.
Three-Dimensional Projection

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Video games make ample use
of three-dimensional projection
to represent three-dimensional
environments on two-dimensional
screens. For example, the game
Black & White uses three-dimensional
projection to create a believable and
navigable three-dimensional world. All
of the depth cues are demonstrated in
these screen shots from the game.
Three-Dimensional Projection 239

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Three-Dimensional Projection** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Three-Dimensional Projection để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Figure-Ground Relationship and Top-Down Lighting Bias
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
