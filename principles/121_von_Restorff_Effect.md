---
name: "von Restorff Effect"
vi: "Hiệu ứng cô lập von Restorff"
summary: "von Restorff Effect (Hiệu ứng cô lập von Restorff): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
---

# Universal Design Principle: von Restorff Effect (Hiệu ứng cô lập von Restorff)

> **Tóm tắt cốt lõi (Summary)**: von Restorff Effect là một nguyên lý thiết kế then chốt thuộc nhóm **learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

von Restorff Effect
A phenomenon of memory in which noticeably different
things are more likely to be recalled than common things.1
The von Restorff effect is the increased likelihood of remembering unique or
distinctive events or objects versus those that are common. The von Restorff effect
is primarily the result of the increased attention given to the distinctive items in a
set, where a set may be a list of words, a number of objects, a sequence of events,
or the names and faces of people. The von Restorff effect occurs when there is
a difference in context (i.e., a stimulus is different from surrounding stimuli) or a
difference in experience (i.e., a stimulus is different from experiences in memory).2
Differences in context occur when something is noticeably different from other
things in the same set or context. For example, in trying to recall a list of characters
such as EZQL4PMBI, people will have heightened recall for the 4 because it is
the only number in the sequence—compare the relative difficulty of recall of the
4 to the T in a similar list, EZQLTPMBI. The difference between the 4 and the text
characters makes the 4 more memorable than the T. Differences in context of this
type explain why unique brands, distinctive packaging, and unusual advertising
campaigns are used to promote brand recognition and product sales—i.e.,
difference attracts attention and is better remembered.
Differences in experience occur when something is noticeably different from past
experience. For example, people often remember major events in their life, such
as their first day of college or their first day at a new job. Differences in experience
also apply to things like atypical words and faces. Unique words and faces are
better remembered than typical words and faces.3
Take advantage of the von Restorff effect by highlighting key elements in a
presentation or design (e.g., bold text). If everything is highlighted, then nothing is
highlighted, so apply the technique sparingly. Since recall for the middle items in
a list or sequence is weaker than items at the beginning or end of a list, consider
using the von Restorff effect to boost recall for the middle items. Unusual words,
sentence constructions, and images are better remembered than their more typical
counterparts, and should be considered to improve interestingness and recall.
See also Highlighting, Serial Position Effects, and Threat Detection.

1 Also known as the isolation effect and
novelty effect.
2 The seminal work on the von Restorff effect is
“Analyse von Vorgangen in Spurenfeld. I.
Über die Wirkung von Bereichsbildung im
Spurenfeld” [Analysis of Processes in the
Memory Trace: On the Effect of Region-
Formation on the Memory Trace] by Hedwig
von Restorff, Psychologische Forschung, 1933,
vol. 18, p. 299–342.
3 Unusual words with unusual spellings are
found in abundance in the Harry Potter books
of J. K. Rowling, and are among the frequently
cited reasons for their popularity with children.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

von Restorff Effect 255
Word List
milk
eggs
bread
lettuce
butter
flour
ostrich
orangutan
penguin
cheese
sugar
ice cream
oranges
apples
coffee
The Chick-fil-A billboards use a
combination of dimensionality and
humor to attract attention and
increase memorability. The billboards
effectively command attention in
visually noisy environments, clearly
and intelligently promote the Chick-
fil-A brand, and are quickly read and
understood. As billboard design goes,
it does not get much better.
The unique paint schemes on certain
Southwest Airlines planes are very
distinct and memorable. The paint
schemes differentiate Southwest
Airlines from their competitors,
promote vacation destinations
and partners, and reinforce their
reputation as a fun, people-centered
airline. This is a photograph of the
Shamu One, a Southwest Airlines
Boeing 737.
Items in the middle of a list or a
sequence are harder to remember
than items at the beginning or end.
However, the middle items can be
made more memorable if they are
different from other items in the set.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **von Restorff Effect** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý von Restorff Effect để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Highlighting, Serial Position Effects, and Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
