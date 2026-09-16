---
name: "Good Continuation"
vi: "Nguyên lý tiếp diễn mượt mà"
summary: "Good Continuation (Nguyên lý tiếp diễn mượt mà): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Good Continuation (Nguyên lý tiếp diễn mượt mà)

> **Tóm tắt cốt lõi (Summary)**: Good Continuation là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Good Continuation
Elements arranged in a straight line or a smooth curve are
perceived as a group, and are interpreted as being more
related than elements not on the line or curve.
Good continuation is one of several principles referred to as Gestalt principles of
perception. It asserts that aligned elements are perceived as a single group or
chunk, and are interpreted as being more related than unaligned elements. For
example, speed markings on a speedometer are easily interpreted as a group
because they are aligned along a linear or circular path.1
The principle of good continuation also explains why lines will generally be
perceived as maintaining their established directions, versus branching or bending
abruptly. For example, two V-shaped lines side by side appear simply as two
V-shaped lines. When one V-shaped line is inverted and the other is placed above
it (forming an X), the shape is interpreted as two opposing diagonal lines instead
of two V-shaped lines—the less abrupt interpretation of the lines is dominant. A
bar graph in which the bars are arranged in increasing or decreasing order so that
the tops of the bars form a continuous line are more easily processed than bar
arrangements in which the tops of the bars form a discontinuous, abrupt line.2
The ability to accurately perceive objects depends largely on the perceptibility
of the corners and sharp curves that make up their shape. When sections of a
line or shape are hidden from view, good continuation leads the eye to continue
along the visible segments. If extensions of these segments intersect with minimal
disruption, the elements along the line will be perceived as related. As the angle of
disruption becomes more acute, the elements will be perceived as less related.3
Use good continuation to indicate relatedness between elements in a design.
Locate elements such that their alignment corresponds to their relatedness, and
locate unrelated or ambiguously related items on different alignment paths. Ensure
that line extensions of related objects intersect with minimum line disruption.
Arrange elements in graphs and displays such that end points of elements form
continuous, rather than abrupt lines.
See also Alignment, Area Alignment, Chunking, Five Hat Racks, and Uniform
Connectedness.
1 The seminal work on good continuation is
“Untersuchungen zür Lehre von der Gestalt,
II” [Laws of Organization in Perceptual
Forms] by Max Wertheimer, Psychologische
Forschung, 1923 , vol. 4, p. 301–350 ,
reprinted in A Source Book of Gestalt
Psychology by Willis D. Ellis (ed.), Routledge
& Kegan Paul, 1999, p. 71–88 . See also
Principles of Gestalt Psychology by Kurt
Koffka, Harcourt Brace, 1935 .
2 See, for example, Elements of Graph Design
by Stephen M. Kosslyn, W. H Freeman and
Company, 1994, p. 7.
3 See, for example, “Convexity in Perceptual
Completion: Beyond Good Continuation” by
Zili Liu, David W. Jacobs, and Ronen Basri,
Vision Research, 1999, vol. 39, p. 4244–4257.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

10
9
8
7
6
5
4
3
2
1
10
9
8
7
6
5
4
3
2
1
Despite the gaps, the jagged line is
still seen as a single object because
the occlusions can be bridged with
minimal disruption.
The first graph is easier to read
than the second because the end
points of its bars form a line that is
more continuous.
The circular alignment of the
increments of this speedometer
make it evident that the numbers
and increments along the lines
belong together.
Good continuation is commonly used
in camouflage. For example, the lines
on zebras continue across one another
when in a herd, making it difficult for
predators to target any one zebra.
Bob Mary Sue 	Jack 	Tim 	Mary 	Jack 	Bob 	Tim Sue
Burritos Eaten
	Burritos Eaten

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Good Continuation** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Good Continuation để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Alignment, Area Alignment, Chunking, Five Hat Racks, and Uniform
Connectedness
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
