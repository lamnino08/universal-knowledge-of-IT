---
name: "Affordance"
vi: "Khả năng biểu đạt công năng"
summary: "Affordance (Khả năng biểu đạt công năng): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - usability
---

# Universal Design Principle: Affordance (Khả năng biểu đạt công năng)

> **Tóm tắt cốt lõi (Summary)**: Affordance là một nguyên lý thiết kế then chốt thuộc nhóm **perception, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Affordance
A property in which the physical characteristics of an
object or environment influence its function.
Objects and environments are better suited for some functions than others. Round
wheels are better suited than square wheels for rolling; therefore, round wheels
are said to better afford rolling. Stairs are better suited than fences for climbing;
therefore, stairs are said to better afford climbing. This is not to say that square
wheels cannot be rolled or fences climbed, rather that the physical characteristics
of round wheels and stairs better afford the functions of rolling and climbing.1
When the affordance of an object or environment corresponds with its intended
function, the design will perform more efficiently and will be easier to use.
Conversely, when the affordance of an object or environment conflicts with its
intended function, the design will perform less efficiently and be more difficult to
use. For example, a door with a handle affords pulling. Sometimes, doors with
handles are designed to open only by pushing—the affordance of the handle
conflicts with the door’s function. Replace the handle with a flat plate, and it now
affords pushing—the affordance of the flat plate corresponds to the way in which
the door can be used. The design is improved.
Images of common physical objects and environments can enhance the usability
of a design. For example, a drawing of a three-dimensional button on a computer
screen leverages our knowledge of the physical characteristics of buttons and,
therefore, appears to afford pressing. The popular “desktop” metaphor used by
computer operating systems is based on this idea—images of common items like
trash cans and folders leverage our knowledge of how those items function in the
real world and, thus, suggest their function in the software environment.2
Whenever possible, you should design objects and environments to afford their
intended function, and negatively afford improper use. For example, stackable
chairs should only stack one way. Mimic familiar objects and environments in
abstract contexts (e.g., software interfaces) to imply the way in which new systems
can be used. When affordances are successfully employed in a design, it will
seem inconceivable that the design could function or be used otherwise.
See also Constraint, Desire Line, Mapping, and Nudge.

1 The seminal work on affordances is “The
Theory of Affordances” by James Gibson,
in Perceiving, Acting, and Knowing by R.
E. Shaw & J. Bransford (Eds), Lawrence
Erlbaum Associates, 1977; and The Ecological
Approach to Visual Perception by James
Gibson, Houghton Mifflin, 1979. A popular
treatment of affordances can be found in The
Design of Everyday Things by Donald Norman,
Doubleday, 1990.
2 Note that the term affordance refers to the
properties of a physical object or environment
only. When images of physical objects or
environments are used (e.g., image of a
button), the images, themselves, do not afford
anything. The knowledge of button affordances
exists in the mind of the perceiver based
on experience with physical buttons—it is
not a property of the image. Therefore, the
affordance is said to be perceived. See, for
example, “Affordances and Design” by Donald
Norman, www.jnd.org.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Affordance 23
Outdoor lighting structures often
afford landing and perching for birds.
Where birds perch, birds poop. This
anti-perch fixture is designed to attach
to such structures and reduce the
perching affordance.
Door affordances frequently conflict,
as shown in the door on the left.
The “push” affordance of the door is
knowable only because of the sign,
which conflicts with the powerful
“pull” affordance of the handle. By
replacing the handle with a flat plate,
the conflict is eliminated and the sign
is superfluous.
With opposing male and female
surfaces and featureless sides,
Legos naturally afford plugging into
one another.
OXO is well known for the handle
designs of their products; shape,
color, and texture combine to create
irresistible gripping affordances.
The recessed footplates and
handlebar orientation of the
Segway Human Transporter
afford one mounting position
for the user—the correct one.
PUSH

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Affordance** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Affordance để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Constraint, Desire Line, Mapping, and Nudge
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
