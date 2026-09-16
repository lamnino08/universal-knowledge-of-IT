---
name: "Threat Detection"
vi: "Phát hiện mối đe dọa (Threat Detection)"
summary: "Threat Detection (Phát hiện mối đe dọa (Threat Detection)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Threat Detection (Phát hiện mối đe dọa (Threat Detection))

> **Tóm tắt cốt lõi (Summary)**: Threat Detection là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Threat Detection
An ability to detect threatening stimuli more efficiently
than nonthreatening stimuli.
People are born with automatic visual detection mechanisms for evolutionarily
threatening stimuli, such as snakes. These threatening stimuli are detected more
quickly than nonthreatening stimuli and are thought to have evolutionary origins;
efficiently detecting threats no doubt provided a selective advantage for our
human ancestors.1
For example, when presented with images containing threatening elements, such
as spiders, and nonthreatening elements, such as flowers, people can locate the
threatening elements more quickly than the non-threatening elements. The search
times are not affected by the location of the threatening element or the number of
distracters surrounding the element. Similarly, people can locate an angry face in
a group of happy or sad faces more quickly than a happy or sad face in a group
of angry faces. The ability to detect evolutionarily threatening stimuli is a function
of perceptual processes that automatically scan the visual field below the level
of conscious awareness. Unlike conscious processing, which is relatively slow
and serial, threat detection occurs quickly and in parallel with other visual and
cognitive processes.2
Almost anything possessing the key threat features of snakes, spiders, and angry
faces can trigger the threat detection mechanism, such as the wavy line of a
snake, the thin legs and large circular body of spiders, and the V-shaped eyebrows
of an angry face. It is reasonable that other general predatory features (e.g.,
forward-looking eyes) will also trigger the threat-detection mechanism given their
evolutionary relevance, but little research of this type has been conducted. In any
event, the sensitivity to certain threat features explains why twigs and garden hoses
often frighten young children, and why people have a general fear of insects that
superficially resemble spiders (e.g., roaches). When people have conscious fears or
phobias of the threatening stimuli, the threat detection ability is more sensitive, and
search times for threatening stimuli are further reduced. Once attention is captured,
threatening stimuli are also better at holding attention than nonthreatening stimuli.
Consider threatening stimuli to rapidly attract attention and imply threat or
foreboding (e.g., designs of markers to keep people away from an area).
Abstracted representations of threat features can trigger threat-detection
mechanisms without the accompanying negative emotional reaction. Therefore,
consider such elements to attract attention in noisy environments, such as a
dense retail shelf display. Achieving a balance between maximum detectability
and minimal negative affect is more art than science, and therefore should be
explored with caution and verified with testing on the target audience.
See also Baby-Face Bias, Freeze-Flight-Fight-Forfeit, Inattentional Blindness, and
Red Effect.

1 The seminal theoretical work on threat
detection in humans is The Principles of
Psychology by William James, Henry Holt and
Company, 1890. While the evidence suggests
innate detection mechanisms for snakes,
spiders, and angry faces, it is probable that
similar detection mechanisms exist for other
forms of threatening stimuli.
2 See “Emotion Drives Attention: Detecting
the Snake in the Grass” by Arne Öhman,
Anders Flykt, and Francisco Esteve, Journal of
Experimental Psychology: General, September
2001, vol. 130(3), p. 466–478; and “Finding
the Face in the Crowd: An Anger Superiority
Effect” by Christine H. Hansen and Ranald
D. Hansen, Journal of Personality and Social
Psychology, 1988, vol. 54, p. 917–924.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Threat Detection 237
Angry faces are more quickly
detected and maintain attention
more effectively than neutral or
happy faces.
Amid the many billboards lining
Houston freeways, the University
of Houston billboard pops out and
commands attention. The design of
the advertisement is certainly clean
and well composed, but its unique
ability to capture and hold attention
may be due to threat detection.
In visually noisy environments,
the average search time for
threatening stimuli is less than for
nonthreatening stimuli.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Threat Detection** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Threat Detection để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Baby-Face Bias, Freeze-Flight-Fight-Forfeit, Inattentional Blindness, and
Red Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
