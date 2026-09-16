---
name: "Legibility"
vi: "Độ dễ phân biệt ký tự (Legibility)"
summary: "Legibility (Độ dễ phân biệt ký tự (Legibility)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - learning
---

# Universal Design Principle: Legibility (Độ dễ phân biệt ký tự (Legibility))

> **Tóm tắt cốt lõi (Summary)**: Legibility là một nguyên lý thiết kế then chốt thuộc nhóm **perception, learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Legibility
The visual clarity of text, generally based on the size,
typeface, contrast, text block, and spacing of the
characters used.
Confusion regarding the research on legibility is as persistent as it is pervasive.
The rapid growth and advancement of modern desktop publishing, Web-based
publishing, and multimedia presentation continue to compound the confusion with
increasing font and layout capabilities, display and print options, and the need to
effectively integrate with other media. The following guidelines address common
issues regarding text legibility.1
Size
For printed text, standard 9- to 12-point type is considered optimal. Smaller
sizes are acceptable when limited to captions and notes. Use larger type for low-
resolution displays and more senior audiences.2
Typeface
There is no performance difference between serif and sans serif typefaces, so
select based on aesthetic preference. Sentence case text should be used for text
blocks. On low-resolution displays, antialiasing the text may marginally improve
legibility, but primarily serves as an aesthetic enhancement of the typeface.3
Contrast
Use dark text on a light background or vice versa. Performance is optimal when
contrast levels between text and background exceed 70 percent. Foreground/
background color combinations generally do not affect legibility as long as you
observe the minimum contrast level, so select based on aesthetic preference.
Patterned or textured backgrounds can dramatically reduce legibility, and should
be avoided.4
Text Blocks
There is no performance difference between justified and unjustified text, so select
based on aesthetic preference. For 9- to 12-point type, a line length of 3 to 5 inches
(8 cm to 13 cm) is recommended, resulting in a maximum of about 10 to 12
words per line, or 35 to 55 characters per line.5
Spacing
For 9- to 12-point type, set leading (spacing between text lines, measured from
baseline to baseline) to the type size plus 1 to 4 points. Proportionally spaced
typefaces are preferred over monospaced.
See also Iconic Representation and Readability.

1 The seminal empirical works on legibility
for print are Bases for Effective Reading,
University of Minnesota Press, 1963; and
Legibility of Print, Iowa State University
Press, 1965, both by Miles A. Tinker. A
comprehensive and elegant contemporary
reference from a typographic perspective is
The Elements of Typographic Style by Robert
Bringhurst, Hartley & Marks (2nd ed.), 1997.
2 Legibility research on low-resolution computer
displays continues to yield mixed results but
generally supports Tinker’s original findings.
However, be conservative to account for lower-
resolution displays.
3 On lower-resolution displays and for type
smaller than 12 point, use sans serif typefaces
without antialiasing. Serifs and antialiasing blur
the characters of smaller type and, therefore,
compromise legibility.
4 Dark text on light backgrounds is preferred.
High-contrast, inverse text can “visually bleed”
to the background and dramatically reduce
legibility. Factors other than legibility should
be considered when selecting foreground/
background color combinations (e.g., color
blindness and fatigue), so select carefully and
test atypical combinations.
5 The speed with which text can be visually
processed is greatest on long text lines (80
characters or more). However, readers prefer
short text lines (35 to 55 characters). Unless
visual processing speed is critical to the design
task, shorter text lines are recommended. See,
for example, “The Effects of Line Length and
Method of Movement on Patterns of Reading
from Screen,” by Mary C. Dyson and Gary J.
Kipping, Visible Language, 1998, vol. 32(2),
p. 150–181.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Legibility 149
Contrast
Serif vs. San Serif
Serif typefaces have small “feet” at the
ends of the letters.
Antialiased vs. Aliased Text
Antialiased text looks smooth because
of pixels added to smooth the transition
between the text color and the
background color. Aliased text looks
jagged because it does not contain these
transition pixels.
Text Cases
This is sentence case
This is Title Case
this is lowercase
THIS IS UPPERCASE
Aligned Right, Ragged Left Text
Soon her eye fell on a little glass
box that was lying under the table: she
opened it, and found in it a very small
cake, on which the words “EAT ME”
were beautifully marked in currants.
Justified Text
Soon her eye fell on a little glass box
that was lying under the table: she
opened it, and found in it a very small
cake, on which the words “EAT ME” were
beautifully marked in currants.
Leading
Leading (rhymes with sledding) is the
amount of vertical space from the
baseline of one line of text to the
baseline of the next line of text. Below,
the type size is 12 points and the
leading is 18 points.
Monospaced vs. Proportionally
Spaced Typefaces
In monospaced typefaces, all characters
assume the same amount of horizontal
space. In proportionally spaced
typefaces, characters assume variable
amounts of horizontal space, depending
on the width of the actual character
and the relationships among groups
of characters.
Aligned Left, Ragged Right Text
Soon her eye fell on a little glass box
that was lying under the table: she
opened it, and found in it a very small
cake, on which the words “EAT ME ”
were beautifully marked in currants.
Uppercase vs. Mixed Case
People recognize words by letter groups
and shapes. Uppercase text is more
difficult to read than sentence case
and title case because the shapes of
uppercase words are all rectangular.
This is 9-point Trade Gothic 	This is 10-point Trade Gothic 	This is 12-point Trade Gothic
Size
Textblocks	Textblocks
Spacing
Typeface
Baseline
Leading
Baseline

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Legibility** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Legibility để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Iconic Representation and Readability
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
