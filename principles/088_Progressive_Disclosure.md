---
name: "Progressive Disclosure"
vi: "Tiết lộ thông tin lũy tiến"
summary: "Progressive Disclosure (Tiết lộ thông tin lũy tiến): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - usability
---

# Universal Design Principle: Progressive Disclosure (Tiết lộ thông tin lũy tiến)

> **Tóm tắt cốt lõi (Summary)**: Progressive Disclosure là một nguyên lý thiết kế then chốt thuộc nhóm **learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Progressive Disclosure
A strategy for managing information complexity in which
only necessary or requested information is displayed at
any given time.
Progressive disclosure involves separating information into multiple layers and
only presenting layers that are necessary or relevant. It is primarily used to prevent
information overload, and is employed in computer user interfaces, instructional
materials, and the design of physical spaces.1
Progressive disclosure keeps displays clean and uncluttered and helps people
manage complexity without becoming confused, frustrated, or disoriented. For
example, infrequently used controls in software interfaces are often concealed in
dialog boxes that are invoked by clicking a More button. People who do not need
to use the controls never see them. For more advanced users, the options are
readily available. In either case, the design is simplified by showing only the most
frequently required controls by default, and making additional controls available
on request.2
Learning efficiency benefits greatly from the use of progressive disclosure.
Information presented to a person who is not interested or ready to process it
is effectively noise. Information that is gradually and progressively disclosed to
a learner as they need or request it is better processed and perceived as more
relevant. The number of errors is significantly reduced using this method, and
consequently the amount of time and frustration spent recovering from errors is
also reduced.3
Progressive disclosure is also used in the physical world to manage the perception
of complexity and activity. For example, progressive disclosure is found in the
design of entry points for modern theme park rides. Exceedingly long lines not
only frustrate people in line, but also discourage new people from the ride. Theme
park designers progressively disclose discrete segments of the line (sometimes
supplemented with entertainment), so that no one, in or out of the line, ever sees
the line in its entirety.
Use progressive disclosure to reduce information complexity, especially when
people interacting with the design are novices or infrequent users. Hide
infrequently used controls or information, but make them readily available through
some simple operation, such as pressing a More button. Progressive disclosure
is also an effective method for leading people through complex procedures, and
should be considered when such procedures are a part of a design.
See also Chunking, Errors, Layering, and Performance Load.

1 The seminal applied work on progressive
disclosure is the user interface for the Xerox
Star computer. See “The Xerox ‘Star’: A
Retrospective” by Jeff Johnson and Teresa
L. Roberts, William Verplank, David C. Smith,
Charles Irby, Marian Beard, Kevin Mackey,
in Human Computer Interaction: Toward the
Year 2000 by Ronald M. Baecker, Jonathan
Grudin, William A. S. Buxton, Saul Greenberg,
Morgan Kaufman Publishers, 1995, p. 53–70.
2 A common mistake is to present all available
information and options at once with the
rationale that it reduces kinematic load. Since
progressive disclosure affects only infrequently
used elements and elements for which a
person may not be ready, it will generally have
minimal effect on kinematic load. Conversely,
presenting everything at once will significantly
increase cognitive load.
3 See, for example, “Training Wheels in a User
Interface” by John M. Carroll and Caroline
Carrithers, Communications of the ACM, 1984,
vol. 27(8), p. 800–806; and The Nurnberg
Funnel by John M. Carroll, MIT Press, 1990.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

ARE YOU READY FOR…
JUST 10 MINUTES AWAY
Progressive disclosure is commonly
used in software to conceal
complexity. In this dialog box, basic
search functionality is available by
default. However, more complex
search functionality is available upon
request by clicking More Choices.
Theme park rides often have very long
lines—so long that seeing the lines in
their entirety would scare away many
would-be visitors. Therefore, modern
theme park rides progressively
disclose the length of the line, so that
only small segments of the line can
be seen from any particular vantage
point. Additional distractions are
provided in the form of video
screens, signage, and partial
glimpses of people on the ride.
Progressive Disclosure 189
Status signs
indicate wait time.
Low walls allow visitors near the
end of the line to see they are
getting close to the end.
Windows allow visitors
at the end of the line
to see the ride.
Video screens entertain
visitors while they wait.
High walls prevent visitors
at the beginning of the line
from seeing the length of the line.
Find: name 	contains
Fewer Choices
Find
Find:
More Choices 	Cancel
Cancel
Find
Find
Find
Search: on all disks

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Progressive Disclosure** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Progressive Disclosure để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Errors, Layering, and Performance Load
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
