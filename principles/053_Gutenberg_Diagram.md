---
name: "Gutenberg Diagram"
vi: "Sơ đồ Gutenberg"
summary: "Gutenberg Diagram (Sơ đồ Gutenberg): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Gutenberg Diagram (Sơ đồ Gutenberg)

> **Tóm tắt cốt lõi (Summary)**: Gutenberg Diagram là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Gutenberg Diagram
A diagram that describes the general pattern followed by
the eyes when looking at evenly distributed, homogeneous
information.1
The Gutenberg diagram divides a display medium into four quadrants: the primary
optical area at the top left, the terminal area at the bottom right, the strong fallow
area at the top right, and the weak fallow area at the bottom left. According to
the diagram, Western readers naturally begin at the primary optical area and
move across and down the display medium in a series of sweeps to the terminal
area. Each sweep begins along an axis of orientation—a horizontal line created
by aligned elements, text lines, or explicit segments—and proceeds in a left-to-
right direction. The strong and weak fallow areas lie outside this path and receive
minimal attention unless visually emphasized. The tendency to follow this path
is metaphorically attributed to reading gravity—the left-right, top-bottom habit
formed from reading.2
Designs that follow the diagram work in harmony with reading gravity, and return
readers to a logical axis of orientation, purportedly improving reading rhythm
and comprehension. For example, a layout following the Gutenberg diagram
would place key elements at the top left (e.g., headline), middle (e.g., image),
and bottom right (e.g., contact information). Though designs based directly or
indirectly on the Gutenberg diagram are widespread, there is little empirical
evidence that it contributes to improved reading rates or comprehension.
The Gutenberg diagram is likely only predictive of eye movement for heavy text
information, evenly distributed and homogeneous information, and blank pages or
displays. In all other cases, the weight of the elements of the design in concert with
their layout and composition will direct eye movements. For example, if a newspaper
has a very heavy headline and photograph in its center, the center will be the
primary optical area. Familiarity with the information and medium also influences
eye movements. For example, a person who regularly views information presented
in a consistent way is more likely to first look at areas that are often changing (e.g.,
new top stories) than areas that are the same (e.g., the title of a newspaper).
Consider the Gutenberg diagram to assist in layout and composition when the
elements are evenly distributed and homogeneous, or the design contains heavy
use of text. Otherwise, use the weight and composition of elements to lead the eye.
See also Alignment, Entry Point, Progressive Disclosure, and Serial Position Effects.
1 Also known as the Gutenberg rule and the Z
pattern of processing.
2 The seminal work on the Gutenberg diagram is
attributed to the typographer Edmund Arnold,
who is said to have developed the concept in
the 1950s. See, for example, Type & Layout:
How Typography and Design Can Get Your
Message Across or Get in the Way, by Colin
Wheildon, Strathmoor Press, 1995.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Gutenberg Diagram 119
Primary Optical Area
Axis of Orientation
Weak Fallow Area
Terminal Area
Strong Fallow Area
Reading gravity pulls the eyes from
the top-left to the bottom-right of the
display medium. In homogeneous
displays, the Gutenberg diagram
makes compositions interesting
and easy to read. However, in
heterogoneous displays, the Gutenberg
diagram does not apply, and can
constrain composition unnecessarily.
The composition of these pages
illustrates the application of the
Gutenberg diagram. The first page is all
text, and it is, therefore, safe to assume
readers will begin at the top-left and
stop at the bottom-right of the page.
The pull quote is placed between these
areas, reinforcing reading gravity. The
placement of the image on the second
page similarly reinforces reading
gravity, which it would not do if it were
positioned at the top-right or bottom-left
of the page.
The redesign of the Wall Street
Journal leads the eyes of readers,
and does not follow the Gutenberg
diagram. Additionally, recurring
readers of the Wall Street Journal
tend to go to the section they find
most valuable, ignoring the other
elements of the page.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Gutenberg Diagram** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Gutenberg Diagram để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Alignment, Entry Point, Progressive Disclosure, and Serial Position Effects
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
