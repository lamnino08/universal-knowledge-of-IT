---
name: "Iconic Representation"
vi: "Biểu tượng hóa trực quan"
summary: "Iconic Representation (Biểu tượng hóa trực quan): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - usability
---

# Universal Design Principle: Iconic Representation (Biểu tượng hóa trực quan)

> **Tóm tắt cốt lõi (Summary)**: Iconic Representation là một nguyên lý thiết kế then chốt thuộc nhóm **perception, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Iconic Representation
The use of pictorial images to improve the recognition and
recall of signs and controls.
Iconic representation is the use of pictorial images to make actions, objects,
and concepts in a display easier to find, recognize, learn, and remember.
Iconic representations are used in signage, computer displays, and control
panels. They can be used for identification (company logo), serve as a space-
efficient alternative to text (road signs), or to draw attention to an item within an
informational display (error icons appearing next to items in a list). There are four
types of iconic representation: similar, example, symbolic, and arbitrary.1
Similar icons use images that are visually analogous to an action, object, or
concept. They are most effective at representing simple actions, objects, or
concepts, and less effective when the complexity increases. For example, a sign
indicating a sharp curve ahead can be represented by a similar icon (e.g., curved
line). A sign to reduce speed, however, is an action not easily represented by
similar icons.
Example icons use images of things that exemplify or are commonly associated with
an action, object, or concept. They are particularly effective at representing complex
actions, objects, or concepts. For example, a sign indicating the location of an
airport uses an image of an airplane, rather than an image representing an airport.
Symbolic icons use images that represent an action, object, or concept at a higher
level of abstraction. They are effective when actions, objects, or concepts involve
well-established and easily recognizable objects. For example, a door lock control
on a car door uses an image of a padlock to indicate its function, even though the
padlock looks nothing like the actual control.
Arbitrary icons use images that bear little or no relationship to the action, object,
or concept—i.e., the relationship has to be learned. Generally, arbitrary icons
should only be used when developing cross-cultural or industry standards that will
be used for long periods of time. This gives people sufficient exposure to an icon
to make it an effective communication device. For example, the icon for radiation
must be learned, as nothing intrinsic to the image indicates radiation. Those who
work with radiation, however, recognize the symbol all over the world.
Iconic representation reduces performance load, conserves display and control
area, and makes signs and controls more understandable across cultures. Consider
similar icons when representations are simple and concrete. Use example icons
when representations are complex. Consider symbolic icons when representations
involve well-established and recognizable symbols. Consider arbitrary icons when
representations are to be used as standards. Generally, icons should be labeled
and share a common visual motif (style and color) for optimal performance.
See also Chunking, Performance Load, and Picture Superiority Effect.

1 The seminal work in iconic representation is
Symbol Sourcebook by Henry Dreyfuss, Van
Nostrand Reinhold, 1984 . The four kinds of
iconic representation are derived from “Icons
at the Interface: Their Usefulness” by Yvonne
Rogers, Interacting With Computers, vol. 1,
p. 105–118 .

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Iconic Representation 133
Similar
Example
Symbolic
Arbitrary
Right Turn 	Falling Rocks 	Sharp 	Stop
Airport 	Cut 	Basketball 	Restaurant
Electricity 	Water 	Unlock 	Fragile
Collate 	Female 	Radioactive 	Resistor

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Iconic Representation** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Iconic Representation để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Performance Load, and Picture Superiority Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
