---
name: "Chunking"
vi: "Phân nhóm thông tin (Chunking)"
summary: "Chunking (Phân nhóm thông tin (Chunking)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - usability
---

# Universal Design Principle: Chunking (Phân nhóm thông tin (Chunking))

> **Tóm tắt cốt lõi (Summary)**: Chunking là một nguyên lý thiết kế then chốt thuộc nhóm **learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A technique of combining many units of information into a
limited number of units or chunks, so that the information
is easier to process and remember.
The term chunk refers to a unit of information in short-term memory—a string
of letters, a word, or a series of numbers. The technique of chunking seeks
to accommodate short-term memory limits by formatting information into a
small number of units. The maximum number of chunks that can be efficiently
processed by short-term memory is four, plus or minus one. For example, most
people can remember a list of five words for 30 seconds, but few can remember
a list of ten words for 30 seconds. By breaking the list of ten words into multiple,
smaller chunks (e.g., two groups of three words, and one group of four words),
recall performance is essentially equivalent to the single list of five words.1
Chunking is often applied as a general technique to simplify designs. This is a
potential misapplication of the principle. The limits specified by this principle
deal specifically with tasks involving memory. For example, it is unnecessary and
counterproductive to restrict the number of dictionary entries on a page to four
or five. Reference-related tasks consist primarily of scanning for a particular item;
chunking in this case would dramatically increase the scan time and effort, and
yield no benefits.
Chunk information when people are required to recall and retain information, or
when information is used for problem solving. Do not chunk information that is
to be searched or scanned. In environments where noise or stress can interfere
with concentration, consider chunking critical display information in anticipation of
diminished short-term memory capacity. Use the contemporary estimate of 4 ± 1
chunks when applying this technique.2
See also Errors, Mnemonic Device, Performance Load, and Signal-to-Noise Ratio.

1 The seminal work on short-term memory
limits is “The Magical Number Seven, Plus or
Minus Two: Some Limits on Our Capacity for
Processing Information” by George Miller, The
Psychological Review, 1956, vol. 63, p. 81–97.
As made evident by the title of Miller’s paper,
his original estimate for short-term memory
capacity was 7 ± 2 chunks.
2 A readable contemporary reference is Human
Memory: Theory and Practice by Alan
Baddeley, Allyn & Bacon, 1997. Regarding
short-term memory limits, see, for example,
“The Magical Number Four in Short-Term
Memory: A Reconsideration of Mental Storage
Capacity” by Nelson Cowan, Behavioral and
Brain Sciences, 2001, vol. 24, p. 87–114.
Chunking

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Familiar words are easier to remember
and chunk together than unfamiliar
words. Of the two lists, list 1 is easier
to recall.
Large strings of numbers are difficult
to recall. Chunking large strings of
numbers into multiple, smaller strings
can help. Most people can remember
their Social Security number and
frequently called phone numbers.
Chunking 41
292-63-5732 	(704) 555-6791
292635732 	7045556791
This e-learning course by Kaplan
EduNeering makes excellent use
of chunking. Note that the number
of content topics (left gray panel)
observes the appropriate limits, as
do the information chunks on the
topics themselves. Overview and
Challenge are not counted because
they contain organizing information
and quizzes only.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Chunking** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Chunking để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Errors, Mnemonic Device, Performance Load, and Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
