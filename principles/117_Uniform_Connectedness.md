---
name: "Uniform Connectedness"
vi: "Nguyên lý liên kết đồng nhất"
summary: "Uniform Connectedness (Nguyên lý liên kết đồng nhất): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Uniform Connectedness (Nguyên lý liên kết đồng nhất)

> **Tóm tắt cốt lõi (Summary)**: Uniform Connectedness là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Uniform Connectedness
Elements that are connected by uniform visual properties,
such as color, are perceived to be more related than
elements that are not connected.
The principle of uniform connectedness is the most recent addition to the
principles referred to as Gestalt principles of perception. It asserts that elements
connected to one another by uniform visual properties are perceived as a single
group or chunk and are interpreted as being more related than elements that
are not connected. For example, a simple matrix composed of dots is perceived
as columns when common regions or lines connect the dots vertically, and is
perceived as rows when common regions or lines connect the dots horizontally.1
There are two basic strategies for applying uniform connectedness in a design:
common regions and connecting lines. Common regions are formed when
edges come together and bound a visual area, grouping the elements within the
region. This technique is often used to group elements in software and buttons
on television remote controls. Connecting lines are formed when an explicit line
joins elements, grouping the connected elements. This technique is often used
to connect elements that are not otherwise obviously grouped (e.g., not located
closely together) or to imply a sequence.
Uniform connectedness will generally overpower the other Gestalt principles. In
a design where uniform connectedness is at odds with proximity or similarity, the
elements that are uniformly connected will appear more related than either the
proximal or similar elements. This makes uniform connectedness especially useful
when correcting poorly designed configurations that would otherwise be difficult
to modify. For example, the location of controls on a control panel is generally
not easily modified, but a particular set of controls can be grouped by connecting
them in a common region using paint or overlays. In this case, the uniform
connectedness resulting from the common region will overwhelm and correct the
poor control positions.
Use uniform connectedness to visually connect or group elements in a design.
Employ common regions to group text elements and clusters of control elements,
and connecting lines to group individual elements and imply sequence. Consider
this principle when correcting poorly designed control and display configurations.
See also Chunking, Figure-Ground Relationship, and Good Continuation.

1 The seminal work on uniform connectedness
is “Rethinking Perceptual Organization: The
Role of Uniform Connectedness” by Stephen
Palmer and Irvin Rock, 1994, Psychonomic
Bulletin & Review, vol. 1, p. 29–55.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Uniform Connectedness 247
The proximity between unrelated
words (e.g., Chisos and South)
on this rendering of a sign at Big
Bend National Park lends itself to
misinterpretation. Grouping the
related words in a common region
would be a simple way to correct
the sign.
The use of common regions and
connecting lines is a powerful
means of grouping elements and
overwhelming competing cues like
proximity and similarity.
Common regions are frequently
used in software interfaces to group
related controls.
Print
Printer
Name: 	BW Printer Xerox DC 432 	Properties...
Status: 	Ready
Type: 	Xerox DC 440/432/425/420 PS 3
Where: 	66.64.13.240:lp
Comment: 	Print to file
Print Range
All
Pages 	from: 	to:
Selection
Copies
Number of Copies
Collate
OK 	Cancel

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Uniform Connectedness** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Uniform Connectedness để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Figure-Ground Relationship, and Good Continuation
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
