---
name: "Errors"
vi: "Quản lý và phòng ngừa lỗi (Errors)"
summary: "Errors (Quản lý và phòng ngừa lỗi (Errors)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - decision
---

# Universal Design Principle: Errors (Quản lý và phòng ngừa lỗi (Errors))

> **Tóm tắt cốt lõi (Summary)**: Errors là một nguyên lý thiết kế then chốt thuộc nhóm **usability, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

An action or omission of action yielding an unintended result.
Most accidents are thought to be caused by what is referred to as human error,
yet most accidents are actually due to design errors rather than errors of human
operation. An understanding of the causes of errors suggests specific design
strategies that can greatly reduce their frequency and severity. There are two basic
types of errors: slips and mistakes.1
Slips are sometimes referred to as errors of action or errors of execution, and
occur when an action is not what was intended. For example, a slip occurs when
a person dials a frequently dialed phone number when intending to dial a different
number. Slips are the result of automatic, unconscious processes, and frequently
result from a change of routine or an interruption of an action. For example, a
person forgets their place in a procedure when interrupted by a phone call.2
Minimize slips by providing clear feedback on actions. Make error messages
clear, and include the consequences of the error, as well as corrective actions, if
possible. Position controls to prevent accidental activation of functions that may
have detrimental consequences. When this is not possible, use confirmations
to interrupt the flow and verify the action. Consider the use of affordances and
constraints to influence actions.
Mistakes are sometimes referred to as errors of intention or errors of planning, and
occur when an intention is inappropriate. For example, a mistake occurs when a
nurse interprets an alarm incorrectly and then administers the incorrect medicine.
Mistakes are caused by conscious mental processes, and frequently result from
stress or decision-making biases. For example, a person is biased to select only
from visible options.
Minimize mistakes by increasing situational awareness and reducing
environmental noise. Make key indicators and controls visible within one eyespan
whenever possible. Reduce stress and cognitive load by minimizing the auditory
and visual noise. Provide just enough feedback to accomplish warnings and other
functions, and no more. Consider the use of confirmations that require multiple
steps to verify the intention of highly critical tasks. Train on error recovery and
troubleshooting, emphasizing communication with other team members.
Finally, always incorporate the principle of forgiveness into a design. Forgiveness
refers to the use of design elements to reduce the frequency and severity of errors
when they occur, enhancing the design’s safety and usability.
See also Affordance, Confirmation, Constraint, and Forgiveness.
1 The seminal work on errors is “Categorization
of Action Slips” by Donald A. Norman,
Psychological Review, 1981, vol. 88, p. 1–15;
and Absent Minded? The Psychology of Mental
Lapses and Everyday Errors by James Reason
and Klara Mycielska, Prentice-Hall, 1982.
2 Note that there are many different error
taxonomies. A nice review and discussion
regarding the various taxonomies is found in
Human Error by James Reason, Cambridge
University Press, 1990 . A very readable
and interesting treatment of human error
is Set Phasers on Stun and Other True
Tales of Design, Technology, and Human
Error by Steven Casey, Aegean Publishing
Company, 1998 .
Errors

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Errors 83
Changes to repetitive tasks or habits
Provide clear and distinctive feedback
Use confirmations for critical tasks
Consider constraints, affordances, and mappings
Confirmations are useful for disrupting behaviors and
verifying intent
Distractions and interruptions
Provide clear orientation and status cues
Use highlighting to focus attention
Use alarms to attract attention for critical situations
Clear orientation and status cues are useful for enabling
the easy resumption of interrupted procedures
Incomplete or ambiguous feedback
Improve situational awareness
Provide clear and distinctive feedback
Track and display historical system behaviors
Historical displays are useful for revealing trends that are
not detectable in point-in-time displays
Stress, decision biases, and overconfidence
Minimize information and environmental noise
Use checklists and decision trees
Train on error recovery and troubleshooting
Decision trees and checklists are useful decision-making
and troubleshooting tools, especially in times of stress
Lack of knowledge and poor communication
Use memory and decision aids
Standardize naming and operational conventions
Train using case studies and simulations
Memory mnemonics are useful strategies for remembering
critical information in emergency situations
Two Types of Slips
Three Types of Mistakes
CANCEL 	BACK 	NEXT
YES
NO
Does the
computer
start from its
hardrive?
Is the new
software icon
on the
desktop?
Does the
computer
start from a
CD-ROM?
How to use a fire extinguisher
P 	pull the pin
A 	aim the hose at the flame
S 	squeeze the trigger
S 	sweep hose from side to side
YES
NO
YES
NO
DANGER
NORMAL
DANGER
time
Action
Attention
Perception
Decision
Knowledge 
temperature
Do you want to
save the changes
to your document
before closing?
Software Instalation
Your Name
Your Company Name
Serial Number
Step 1 2 3 4 5
CAUSES
SOLUTIONS
CAUSES
SOLUTIONS
CAUSES
SOLUTIONS
CAUSES
SOLUTIONS
CAUSES
SOLUTIONS
EXAMPLE
EXAMPLE
EXAMPLE
EXAMPLE
EXAMPLE
No 	Yes

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Errors** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Errors để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Confirmation, Constraint, and Forgiveness
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
