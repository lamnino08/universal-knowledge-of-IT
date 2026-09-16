---
name: "Inattentional Blindness"
vi: "Mù do không chú ý (Inattentional Blindness)"
summary: "Inattentional Blindness (Mù do không chú ý (Inattentional Blindness)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Inattentional Blindness (Mù do không chú ý (Inattentional Blindness))

> **Tóm tắt cốt lõi (Summary)**: Inattentional Blindness là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Inattentional Blindness
The failure to cognitively process a stimulus that is
presented in clear view, leaving the observer without any
awareness or memory of the stimulus.1
When focused on performing a task, observers are often blind to stimuli that
are literally presented right before their eyes. For example, in 1972, an Eastern
Airlines cockpit crew noticed that a landing gear indicator failed to light. They
became so fixated on the cause that they failed to notice their loss in altitude or
respond to ground alarms. The resulting crash killed more than 100 people. In
2001, a submarine commander looked through the periscope and saw no nearby
ships. He ordered the submarine to rapidly surface and unwittingly crashed into
another ship directly overhead. The ship overturned, killing nine people. These
types of occurrences are common, and are not restricted to catastrophic incidents.
It is inattentional blindness that enables many of the tricks and misdirections
employed by magicians and illusionists. Inattentional blindness is one reason
talking on a cell phone while driving is unsafe — the eyes may be on the road, but
the mind is often elsewhere. In any situation where people fix their attention on a
task, they will be blind to stimuli that are unexpected and unrelated to the task.2
How does one capture the attention of a person once he or she is focused on a
task? It isn’t easy. Typically, being very different is a great way to capture attention.
However, when people focus their attention on a certain kind of stimulus, being
very different actually makes it less likely that a second stimulus will be noticed.
For example, in 1996, Pennsylvania highway workers actually paved over a dead
deer — they didn’t see it. It seems reasonable to think that a surprise such as
seeing a deer in the road would have captured the workers’ attention, but again,
counterintuitively, when people are task-focused, unexpected stimuli are actually
worse at getting noticed than anticipated stimuli. When people are in this focused
state, roughly 50 percent will be functionally blind to stimuli not related to the
task. So, what does get noticed? Stimuli that are relevant to the goal (e.g., a
shopper seeking a certain brand of soda will likely notice other soda bottles, but
not dishwasher soap bottles), stimuli expressed through different modalities (e.g.,
auditory versus visual stimuli), faces — whether familiar or anonymous — seem
effective at capturing attention, personally relevant stimuli (e.g., a person’s name),
and threat stimuli (e.g., snakes).3
Consider inattentional blindness in all contexts where attention is key, including
security, safety, product design, retail, and advertising. Given the robustness of
the effect, the best strategy is to create or alter tasks to focus attention on desired
stimuli (e.g., receiving a coupon book prior to visiting a store can predefine the
shopping targets ahead of time). When trying to draw attention away from one
stimulus to another, consider semantically similar stimuli, alternative modalities,
faces, personal names, and threat stimuli.
See also Immersion, Interference Effects, and Threat Detection.
1 Also known as perceptual blindness.
2 The seminal work on inattentional blindness
is Inattentional Blindness by Arien Mack
and Irvin Rock, The MIT Press, 1998.
See also “Gorillas in Our Midst: Sustained
Inattentional Blindness for Dynamic Events”
by Daniel Simons and Christopher Chabris,
Perception, 1999, vol. 28(9), p. 1059–1074;
and “Selective Looking: Attending to Visually
Specified Events” by Ulric Neisser and Robert
Becklen, Cognitive Psychology, 1975, vol. 7,
p. 480–494.
3 See, for example, “What You See Is What You
Set: Sustained Inattentional Blindness and
the Capture of Awareness” by Steven Most,
Brian Scholl, Erin Clifford, et al., Psychological
Review, 2005, vol. 112(1), p. 217–242.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Inattentional Blindness 137
In a now classic experiment on
inattentional blindness, Daniel Simons
and Christopher Chabris showed
subjects a short video of two teams
of students tossing a basketball and
moving about quickly. Subjects were
instructed to count the number of
times the team in the white shirts
passed the basketball, a challenging
task given all of the movement. In the
middle of the video, a student in a
gorilla costume strolls to the center of
the screen, beats her chest, and then
strolls off the screen. Roughly half of
the subjects in the experiment did not
notice the gorilla.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Inattentional Blindness** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Inattentional Blindness để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Immersion, Interference Effects, and Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
