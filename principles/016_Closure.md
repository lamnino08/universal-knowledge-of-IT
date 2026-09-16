---
name: "Closure"
vi: "Nguyên lý đóng kín (Closure)"
summary: "Closure (Nguyên lý đóng kín (Closure)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Closure (Nguyên lý đóng kín (Closure))

> **Tóm tắt cốt lõi (Summary)**: Closure là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A tendency to perceive a set of individual elements as
a single, recognizable pattern, rather than multiple,
individual elements.
The principle of closure is one of a number of principles referred to as Gestalt
principles of perception. It states that whenever possible, people tend to perceive
a set of individual elements as a single, recognizable pattern, rather than
multiple, individual elements. The tendency to perceive a single pattern is so
strong that people will close gaps and fill in missing information to complete the
pattern if necessary. For example, when individual line segments are positioned
along a circular path, they are first perceived holistically as a circle, and then as
comprising multiple, independent elements. The tendency to perceive information
in this way is automatic and subconscious; it is likely a function of an innate
preference for simplicity over complexity, and pattern over randomness.1
Closure is strongest when elements approximate simple, recognizable patterns,
such as geometric forms, and are located near one another. When simple,
recognizable patterns are not easily perceived, designers can create closure
through transitional elements (e.g., subtle visual cues that help direct the eye
to find the pattern). Generally, if the energy required to find or form a pattern is
greater than the energy required to perceive the elements individually, closure will
not occur.
The principle of closure enables designers to reduce complexity by reducing
the number of elements needed to organize and communicate information. For
example, a logo design that is composed of recognizable elements does not need
to complete many of its lines and contours to be clear and effective. Reducing the
number of lines in the logo not only reduces its complexity, but it makes the logo
more interesting to look at—viewers subconsciously participate in the completion
of its design. Many forms of storytelling leverage closure in a similar way. For
example, in comic books, discrete scenes in time are presented to readers, who
then supply what happens in between. The storyline is a unique combination of
information provided by the storyteller, and information provided by the reader.2
Use closure to reduce the complexity and increase the interestingness of designs.
When designs involve simple and recognizable patterns, consider removing or
minimizing the elements in the design that can be supplied by viewers. When
designs involve more complex patterns, consider the use of transitional elements
to assist viewers in finding or forming the pattern.
See also Good Continuation, Law of Prägnanz, and Proximity.

1 The seminal work on closure is
“Untersuchungen zür Lehre von der Gestalt,
II” [Laws of Organization in Perceptual
Forms] by Max Wertheimer, Psychologische
Forschung, 1923, vol. 4, p. 301–350, reprinted
in A Source Book of Gestalt Psychology by
Willis D. Ellis (ed.), Routledge & Kegan Paul,
1999, p. 71–88.
2 See, for example, Understanding Comics: The
Invisible Art by Scott McCloud, Kitchen Sink
Press, 1993.
Closure

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The elements are perceived holistically
as a single pattern first (circle), and
then as individual elements.
Elements in text and graphics can
be minimized to allow viewers to
participate in the completion of
the pattern. The result is a more
interesting design.
Series images are understood as
representing motion because people
supply the information in between
the images.
Closure 45

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Closure** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Closure để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Good Continuation, Law of Prägnanz, and Proximity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
