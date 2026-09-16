---
name: "Similarity"
vi: "Nguyên lý tương đồng (Similarity)"
summary: "Similarity (Nguyên lý tương đồng (Similarity)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Similarity (Nguyên lý tương đồng (Similarity))

> **Tóm tắt cốt lõi (Summary)**: Similarity là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Similarity
Elements that are similar are perceived to be more related
than elements that are dissimilar.
The principle of similarity is one of several principles referred to as Gestalt
principles of perception. It asserts that similar elements are perceived as a
single group or chunk, and are interpreted as being more related than dissimilar
elements. For example, a simple matrix comprising alternating rows of dots and
squares will be interpreted as a set of rows only, because the similar elements
group together to form horizontal lines. A complex visual display is interpreted as
having different areas and types of information depending on the similarity of color,
size, and shape of its elements; similar elements are interpreted as being relevant
to one another.1
The grouping resulting from similarity reduces complexity and reinforces the
relatedness of design elements. Conversely, a lack of similarity results in the
perception of multiple, disparate chunks, and reinforces differences among the
elements. Certain kinds of similarity work better than others for different situations.
Similarity of color results in the strongest grouping effect; it is strongest when the
number of colors is small, and is decreasingly effective as the number of colors
increases. Similarity of size is effective when the sizes of elements are clearly
distinguishable from one another, and is an especially appropriate grouping
strategy when the size of elements has additional benefits (e.g., large buttons
are easier to press). Similarity of shape is the weakest grouping strategy; it is
best used when the color and size of other elements is uniform, or when used in
conjunction with size or color.2
Use similarity to indicate relatedness among elements in a design. Represent
elements such that their similarity corresponds to their relatedness, and represent
unrelated or ambiguously related items using different colors, sizes, and shapes.
Use the fewest colors and simplest shapes possible for the strongest grouping
effects, ensuring that elements are sufficiently distinct to be easily detectable.
See also Chunking, Inattentional Blindness, Mimicry, and Self-Similarity.

1 The seminal work on similarity is
“Untersuchungen zür Lehre von der Gestalt, II”
[Laws of Organization in Perceptual Forms] by
Max Wertheimer, Psychologische Forschung,
1923, vol. 4, p. 301–350, reprinted in A Source
Book of Gestalt Psychology by Willis D. Ellis
(ed.), Routledge & Kegan Paul, 1999, p. 71–88.
See also Principles of Gestalt Psychology by
Kurt Koffka, Harcourt Brace, 1935.
2 Note that a significant portion of the population
is color blind, limiting the strategy of using color
alone. Therefore, consider using an additional
grouping strategy when using color.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Similarity 227
This remote control uses color,
size, and shape to group functions.
Note the relationship between the
anticipated frequency of use of
the buttons and their relative size
and shape.
Similarity is commonly used in
camouflage. For example, the mimic
octopus can assume the color,
pattern, and approximate form of one
of its fiercest predators—the highly
poisonous sole fish—as well as
many other marine organisms.
Similarity among elements influences
how they are grouped—here by
color, size, and shape. Note the
strength of color as a grouping
strategy relative to size and shape.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Similarity** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Similarity để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Inattentional Blindness, Mimicry, and Self-Similarity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
