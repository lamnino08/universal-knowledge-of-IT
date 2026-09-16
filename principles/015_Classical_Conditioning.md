---
name: "Classical Conditioning"
vi: "Phản xạ có điều kiện cổ điển"
summary: "Classical Conditioning (Phản xạ có điều kiện cổ điển): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - appeal
---

# Universal Design Principle: Classical Conditioning (Phản xạ có điều kiện cổ điển)

> **Tóm tắt cốt lõi (Summary)**: Classical Conditioning là một nguyên lý thiết kế then chốt thuộc nhóm **learning, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A technique used to associate a stimulus with an
unconscious physical or emotional response.
Classical conditioning was the first type of learning to be studied by behavioral
psychologists. Lab workers discovered the technique when they noticed that dogs
in the laboratory began salivating as soon as they entered the room. Because
the lab workers feed the dogs, their presence (neutral stimulus) had become
associated with food (trigger stimulus), and, therefore, elicited the same response
as the food itself (salivation). Similar behaviors are seen in fish when they surface
at the sight of an approaching person, or in cats when they come running at the
sound of a can opener.1
Classical conditioning is commonly used in animal training (e.g., associating
chemical traces of TNT with sugar water to train bees to detect bombs), behavior
modification in people (e.g., associating smoking with aversive images or tastes),
and marketing and advertising (i.e., associating products or services with attractive
images or feelings). For example, television and magazine advertising firms use
classical conditioning frequently to associate products and services with specific
thoughts and feelings. Images of attractive people stimulate reward centers in the
brain, and condition positive associations with products, services, and behaviors.
Conversely, disturbing images of extreme violence or injury stimulate pain centers
in the brain, and condition negative associations with products, services, and
behaviors. Human emotions condition quickly and easily in this way, particularly
when the association is negative. In a classic experiment, a young child was
exposed to a white rat accompanied by a loud noise. The child not only grew
to fear the white rat (which he did not fear previously), but other furry things
as well (e.g., fur coats). Many phobias are caused by this type of association.
For example, many children become anxious when visiting the dentist because
previous experiences have been painful—dentists often give children treats in an
attempt to reverse this association.2
Use classical conditioning to influence the appeal of a design or influence specific
kinds of behaviors. Repeated pairings of a design with a trigger stimulus will
condition an association over time. Examples of positive trigger stimuli include
anything that causes pleasure or evokes a positive emotional response—a picture
of food, the sound of a drink being poured, images of attractive people. Examples
of negative trigger stimuli include anything that causes pain or evokes a negative
emotional response—physical pain of a vaccination, an embarrassing experience,
or images of extreme pain and violence.
See also Exposure Effect, Operant Conditioning, Shaping, and Veblen Effect.

Classical Conditioning
1 The seminal work in classical conditioning is
Conditioned Reflexes: An Investigation of the
Physiological Activity of the Cerebral Cortex by
Ivan Pavlov, 1927 (translated and edited by G.
V. Anrep, Dover Publications, 1984).
2 See “Conditioned Emotional Reactions” by
John B. Watson and Rosalie Rayner, Journal
of Experimental Psychology, 1920, vol. 3(1),
p. 1–14; and “Reward Value of Attractiveness
and Gaze” by Knut K. W. Kampe, Chris D.
Frith, Raymond J. Dolan, and Uta Frith,
Nature, 2001, v. 413, p. 589.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

This poster features before and after
images of Jacqueline Saburido, a
20-year old college student who was
hit by a drunk driver. It effectively
associates the strong negative
emotional reaction evoked by
Jacqueline’s injuries with the behavior
that caused them.
Classical Conditioning 43

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Classical Conditioning** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Classical Conditioning để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Exposure Effect, Operant Conditioning, Shaping, and Veblen Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
