---
name: "Fibonacci Sequence"
vi: "Dãy số Fibonacci"
summary: "Fibonacci Sequence (Dãy số Fibonacci): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Fibonacci Sequence (Dãy số Fibonacci)

> **Tóm tắt cốt lõi (Summary)**: Fibonacci Sequence là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A sequence of numbers in which each number is the sum
of the preceding two.
A Fibonacci sequence is a sequence of numbers in which each number is the
sum of the two preceding numbers (e.g., 1, 1, 2, 3, 5, 8, 13). Patterns exhibiting
the sequence are commonly found in natural forms, such as the petals of flowers,
spirals of galaxies, and bones in the human hand. The ubiquity of the sequence in
nature has led many to conclude that patterns based on the Fibonacci sequence
are intrinsically aesthetic and, therefore, worthy of consideration in design.1
Fibonacci patterns are found in many classic works, including classic poetry,
art, music, and architecture. For example, it has been argued that Virgil used
Fibonacci sequences to structure the poetry in the Aeneid. Fibonacci sequences
are found in the musical compositions of Mozart’s sonatas and Beethoven’s Fifth
Symphony. Le Corbusier meshed key measures of the human body and Fibonacci
sequences to develop the Modulor, a classic system of architectural propotions and
measurements to aid designers in achieving practical and harmonious designs.2
Fibonacci sequences are generally used in concert with the golden ratio, a
principle to which it is closely related. For example, the division of any two adjacent
numbers in a Fibonacci sequence yields an approximation of the golden ratio.
Approximations are rough for early numbers in the sequence but increasingly
accurate as the sequence progresses. As with the golden ratio, debate continues as
to the aesthetic value of Fibonacci patterns. Are such patterns considered aesthetic
because people find them to be more aesthetic or because people have been
taught to believe they are aesthetic? Research on the aesthetics of the golden ratio
tends to favor the former, but little empirical research exists on the aesthetics of
non-golden Fibonacci patterns.3
The Fibonacci sequence continues to be one of the most influential patterns
in mathematics and design. Consider Fibonacci sequences when developing
interesting compositions, geometric patterns, and organic motifs and contexts,
especially when they involve rhythms and harmonies among multiple elements.
Do not contrive designs to incorporate Fibonacci sequences, but also do not
forego opportunities to explore Fibonacci relationships when other aspects of the
design are not compromised.
See also Aesthetic-Usability Effect, Golden Ratio, and Most Average Facial
Appearance Effect.
1 The seminal work on the Fibonacci sequence
is Liber Abaci [Book of the Abacus] by
Leonardo of Pisa, 1202. Contemporary seminal
works include The Geometry of Art and Life
by Matila Ghyka, Dover Publications, 1978
[1946]; Elements of Dynamic Symmetry by Jay
Hambidge, Dover Publications, 1978 [1920].
2 See, for example, Structural Patterns and
Proportions in Virgil’s Aeneid by George Eckel
Duckworth, University of Michigan Press,
1962; and “Did Mozart Use the Golden
Section?” by Mike May, American Scientist,
March-April 1996; and Le Modulor by Le
Corbusier, Birkhauser, 2000 [1948].
3 “All That Glitters: A Review of Psychological
Research on the Aesthetics of the Golden
Section” by Christopher D. Green, Perception,
1995, vol. 24, p. 937–968.
Fibonacci Sequence

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1,829
1,397
698
698
432
266
102
165
63
63
39
102
165
266
432
1,130
0 	0
863
863
534
534
330
330
204
204
126
126
78
78
48
2,260
Millimeters
Fibonacci Sequence 95
Le Corbusier derived two Fibonacci
sequences based on key features
of the human form to create the
Modulor. The sequences purportedly
represent a set of ideal measurements
to aid designers in achieving practical
and harmonious proportions in design.
Golden ratios were calculated by
dividing each number in the sequence
by its preceding number (indicated by
horizontal lines).

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Fibonacci Sequence** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Fibonacci Sequence để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Aesthetic-Usability Effect, Golden Ratio, and Most Average Facial
Appearance Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
