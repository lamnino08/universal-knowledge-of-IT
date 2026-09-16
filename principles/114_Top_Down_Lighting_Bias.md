---
name: "Top-Down Lighting Bias"
vi: "Thiên kiến ánh sáng từ trên xuống"
summary: "Top-Down Lighting Bias (Thiên kiến ánh sáng từ trên xuống): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - appeal
---

# Universal Design Principle: Top-Down Lighting Bias (Thiên kiến ánh sáng từ trên xuống)

> **Tóm tắt cốt lõi (Summary)**: Top-Down Lighting Bias là một nguyên lý thiết kế then chốt thuộc nhóm **perception, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Top-Down Lighting Bias
A tendency to interpret shaded or dark areas of an object
as shadows resulting from a light source above the object.1
Humans are biased to interpret objects as being lit from a single light source from
above. This bias is found across all age ranges and cultures, and likely results
from humans evolving in an environment lit from above by the Sun. Had humans
evolved in a solar system with more than one sun, the bias would be different.
As a result of the top-down lighting bias, dark or shaded areas are commonly
interpreted as being farthest from the light source, and light areas are interpreted
as being closest to the light source. Thus, objects that are light at the top and
dark at the bottom are interpreted as convex, and objects that are dark at the top
and light at the bottom are interpreted as concave. In each case, the apparent
depth increases as the contrast between light and dark areas increases. When
objects have ambiguous shading cues the brain switches back and forth between
concave and convex interpretation.2
The top-down lighting bias can also influence the perception of the naturalness
or unnaturalness of familiar objects. Objects that are depicted with top-down
lighting look natural, whereas familiar objects that are depicted with bottom-up
lighting look unnatural. Designers commonly exploit this effect in order to create
scary or unnatural looking images. Interestingly, there is evidence that objects look
most natural and are preferred when lit from the top-left, rather than from directly
above. This effect is stronger for right-handed people than left-handed people,
and is a common technique of artists and graphic designers. For example, in a
survey of over two hundred paintings taken from the Louvre, the Prado, and the
Norton Simon Museums, more than 75 percent were lit from the top left. Top-left
lighting is also commonly used in the design of icons and controls in computer
software interfaces.3
The top-down lighting bias plays a significant role in the interpretation of depth
and naturalness, and can be manipulated in a variety of ways by designers. Use a
single top-left light source when depicting natural-looking or functional objects or
environments. Explore bottom-up light sources when depicting unnatural-looking
or foreboding objects or environments. Use the level of contrast between light and
dark areas to vary the appearance of depth.
See also Figure-Ground Relationship, Iconic Representation, Three-Dimensional
Projection, and Uncanny Valley.

1 Also known as top-lighting preference and
lit-from-above assumption.
2 See “Perception of Shape from Shading,”
Nature, 1988, vol. 331, p. 163–166; and
“Perceiving Shape from Shading,” Scientific
American, vol. 256, p. 76–83, both by
Vilayanur S. Ramachandran.
3 “Where Is the Sun?” by Jennifer Sun and
Pietro Perona, Nature Neuroscience, 1998, vol.
1(3), p. 183–184.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Open
31
/2 Floppy (A:)
Local Disk (C:)
UNTITLED (D:)
CD-RW Drive (E:)
Removable Disk (F:)
Removable Disk (G:)
Removable Disk (H:)
Removable Disk (I:)
File name
Files of type: 	All Formats
Look in: 	My Computer
Open
Cancel
My Recent
Documents
Desktop
My Documents
My Computer
My Network
Places
Two rendered images of the same
person—one lit from top-left and
other from below. The image lit from
top-left looks normal, whereas the
image lit from below looks scary.
Graphical user interfaces generally use
top-left lighting to imply dimensionality of
windows and controls.
The circles lit from above appear
convex, whereas the circles lit
from below appear concave. As
the light source moves from these
positions, the depth cues become
increasingly ambiguous.
SSMac2
temp
System Folder
Documents
Applications (Mac OS 9)
New	document.psd
Photoshop
As a Copy 	Annotations
Alpha Channels 	Spot Colors
Layers
Use Proof Setup: Working CMYK
Embed Color Profile: Adobe RGB (1998)
Save:
Color:
Today, 6:05 PM
Yesterday, 1:29 PM
12/6/02, 4:50 PM
Save As
Save	Cancel
Name 	Date Modified

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Top-Down Lighting Bias** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Top-Down Lighting Bias để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Figure-Ground Relationship, Iconic Representation, Three-Dimensional
Projection, and Uncanny Valley
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
