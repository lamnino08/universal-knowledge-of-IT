---
name: "Depth of Processing"
vi: "Độ sâu xử lý nhận thức"
summary: "Depth of Processing (Độ sâu xử lý nhận thức): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
---

# Universal Design Principle: Depth of Processing (Độ sâu xử lý nhận thức)

> **Tóm tắt cốt lõi (Summary)**: Depth of Processing là một nguyên lý thiết kế then chốt thuộc nhóm **learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A phenomenon of memory in which information that is
analyzed deeply is better recalled than information that is
analyzed superficially.1
Thinking hard about information improves the likelihood that the information will
be recalled at a later time. For example, consider two tasks that involve interacting
with and recalling the same information. In the first task, a group of people is
asked to locate a keyword in a list and circle it. In the second task, another group
of people is asked to locate a keyword in a list, circle it, and then define it. After a
brief time, both groups are asked to recall the keywords from the tasks. The group
that performed the second task will have better recall of the keywords because
they had to analyze the keywords at a deeper level than the group in the first task;
they had to think harder about the information.2
This phenomenon of memory results from the two ways in which information
is processed, known as maintenance rehearsal and elaborative rehearsal.
Maintenance rehearsal simply repeats the same kind of analysis that has already
been carried out. For example, people often use maintenance rehearsal when they
repeat a phone number back to themselves to help them remember; no additional
analysis is performed on the phone number. Elaborative rehearsal involves a
deeper, more meaningful analysis of the information. For example, people engage
in elaborative rehearsal when they read a text passage and then have to answer
questions about the meaning of the passage; additional analysis as to word and
sentence meaning require additional thought. Generally, elaborative rehearsal results
in recall performance that is two to three times better than maintenance rehearsal.3
The key determining factors as to how deeply information is processed are the
distinctiveness of the information, the relevance of the information, and the degree
to which the information is elaborated. Distinctiveness refers to the uniqueness
of the information relative to surrounding information and previous experience.
Relevance refers to the degree to which the information is perceived to be
important. The degree of elaboration refers to how much thought is required
to interpret and understand the information. Generally, deep processing of
information that involves these factors will result in the best possible recall and
retention of information.4
Consider depth of processing in design contexts where recall and retention
of information is important. Use unique presentation and interesting activities
to engage people to deeply process information. Use case studies, examples,
and other devices to make information relevant to an audience. Note that deep
processing requires more concentration and effort than mere exposure (e.g.,
classroom lecture), and therefore frequent periods of rest should be incorporated
into the presentation and tasks.
See also Advance Organizer, Mnemonic Device, Picture Superiority Effect, and
von Restorff Effect.
1 Also known as levels-of-processing approach.
2 The seminal work on depth of processing
is “Levels of Processing: A Framework for
Memory Research” by Fergus I. M. Craik
and Robert S. Lockhart, Journal of Verbal
Learning and Verbal Behavior, 1972, vol. 11,
p. 671–684.
3 See, for example, “Depth of Processing and
the Retention of Words in Episodic Memory”
by Fergus I. M. Craik and Endel Tulving,
Journal of Experimental Psychology: General,
1975, vol. 104, p. 268–294.
4 See, for example, “The Self as a Mnemonic
Device: The Role of Internal Cues” by Francis
S. Bellezza, Journal of Personality and Social
Psychology, 1984, vol. 47, p. 506–516.
Depth of Processing

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Depth of Processing 73
Level of Processing
Shallow 	Deep
Text
Text
Images
Text
Images
Questions
The more deeply learners process
information, the better they learn.
Depth of processing is improved
through the use of multiple
presentation media and learning
activities that engage learners
in elaborative rehearsal—as in
this e-learning course by Kaplan
EduNeering.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Depth of Processing** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Depth of Processing để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Advance Organizer, Mnemonic Device, Picture Superiority Effect, and
von Restorff Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
