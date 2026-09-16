---
name: "Storytelling"
vi: "Kể chuyện trong thiết kế (Storytelling)"
summary: "Storytelling (Kể chuyện trong thiết kế (Storytelling)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - appeal
---

# Universal Design Principle: Storytelling (Kể chuyện trong thiết kế (Storytelling))

> **Tóm tắt cốt lõi (Summary)**: Storytelling là một nguyên lý thiết kế then chốt thuộc nhóm **learning, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Storytelling
A method of creating imagery, emotions, and
understanding of events through an interaction between a
storyteller and an audience.
Storytelling is uniquely human. It is the original method of passing knowledge from
one generation to the next, and remains one of the most compelling methods for
richly communicating knowledge. Storytelling can be oral, as in the traditional
telling of a tale; visual, as in an information graph or movie; or textual, as in a
poem or novel. More recently, digital storytelling has emerged, which involves
telling a story using digital media. This might take the form of a computerized slide
show, a digital video, or educational software. A storyteller can be any instrument of
information presentation that engages an audience to experience a set of events.1
Good storytelling experiences generally require certain fundamental elements.
While additional elements can be added to further augment the quality of a story
or storytelling experience, they can rarely be subtracted without detriment. The
fundamental elements are:
• Setting—The setting orients the audience, providing a sense of time and
place for the story.
• Characters—Character identification is how the audience becomes
involved in the story, and how the story becomes relevant.
• Plot—The plot ties events in the story together, and is the channel through
which the story can flow.
• Invisibility—The awareness of the storyteller fades as the audience focuses
on a good story. When engaged in a good movie or book, the existence of
the medium is forgotten.
• Mood—Music, lighting, and style of prose create the emotional tone of
the story.
• Movement—In a good story, the sequence and flow of events is clear and
interesting. The storyline doesn’t stall.
Use storytelling to engage an audience in a design, evoke a specific emotional
response, or provide a rich context to enhance learning. When successfully
employed, an audience will experience and recall the events of the story in a personal
way—it becomes a part of them. This is a phenomenon unique to storytelling.
See also Framing, Immersion, Personas, Stickiness, and Wayfinding.

1 The seminal work on storytelling is Aristotle’s
Poetics. Additional seminal references include,
The Hero with a Thousand Faces by Joseph
Campbell, Princeton University Press, 1960;
and How to Tell a Story; and Other Essays by
Mark Twain, Oxford University Press, 1996.
A nice contemporary reference on visual
storytelling is Graphic Storytelling by Will Eisner,
Poorhouse Press, 1996.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Storytelling 231
Black Granite
Flowing Water
Asymmetric Table
Flowing Water
Events
Cantilevered Table
The Civil Rights Memorial
Southern Poverty Law Center in Montgomery, Alabama
Setting
Milestone events of the civil rights
movement are presented with their
dates and places. The memorial sits
within the greater, historically relevant
context of the Southern Poverty Law
Center in Montgomery, Alabama.
Characters
The civil rights movement is a story
of individual sacrifice toward the
attainment of a greater good. Key
activists and opponents are integral
to the story and are listed by name.
Plot
Events are presented simply and
concisely, listed in chronological
order and aligned along a circular
path. Progress in the civil rights
movement is inferred as cause-effect
relationships between events. No
editorializing—just the facts.
Invisibility
The table is cantilevered to hide its
structure. The black granite is minimal,
providing maximum contrast with
the platinum-inscribed lettering. The
structure is further concealed through
its interaction with water, which
makes it a mirrored surface.
Mood
The table’s asymmetry suggests a
theme of different but equal. The
mirrored surface created by the water
on black granite reveals the story in
union with the reflected image of the
viewer. The sound of water is calming
and healing.
Movement
The flow of water against gravity
suggests the struggle of the civil
rights movement. As the water gently
pours over the edge, the struggle is
overcome. Simile becomes reality as
water rolls down the back wall.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Storytelling** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Storytelling để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Framing, Immersion, Personas, Stickiness, and Wayfinding
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
