---
name: "Hunter-Nurturer Fixations"
vi: "Định hướng giới tính săn bắn - nuôi dưỡng"
summary: "Hunter-Nurturer Fixations (Định hướng giới tính săn bắn - nuôi dưỡng): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Hunter-Nurturer Fixations (Định hướng giới tính săn bắn - nuôi dưỡng)

> **Tóm tắt cốt lõi (Summary)**: Hunter-Nurturer Fixations là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Hunter-Nurturer Fixations
A tendency for male children to be interested in hunting-
related objects and activities, and female children to be
interested in nurturing-related objects and activities.
There are a number of innate cognitive-behavioral differences between males and
females, one of which is early childhood play preferences. Male children tend to
engage in play activities that emulate hunting-related behaviors, whereas female
children tend to engage in play activities that emulate nurturing-related behaviors.
Although such preferences were long thought to be primarily a function of social
and environmental factors, research increasingly favors a more biologically based
explanation. For example, that male children tend to prefer stereotypically male
toys (e.g., cars) and females tend to prefer stereotypically female toys (e.g., dolls)
has long been established. However, in studies where male and female vervet
monkeys are presented with the same human toys, the male vervets prefer to play
with the male toys and the female vervets prefer to play with the female toys. This
suggests a deeply rooted, biologically based gender bias for certain play behaviors.1
Like play behaviors in other animals, these early childhood fixations likely had
adaptive significance in preparing our hunter-gatherer ancestors for survival:
male children for hunting and female children for child rearing. Though these
fixations are essentially vestigial in modern society, they continue to influence our
preferences and behaviors from early childhood through adolescence.
Hunter fixation is characterized by activities involving:
• Object movement and location
• Weapons and tools
• Hunting and fighting
• Predators
• Physical play
Nurturer fixation is characterized by activities involving:
• Form and colors
• Facial expressions and interpersonal skills
• Nurturing and caretaking
• Babies
• Verbal play
Consider hunter-nurturer fixations in the design of objects and environments for
children. When targeting male children, incorporate elements that involve object
movement and tracking, angular forms, predators, and physical play. When
targeting female children, incorporate elements that involve aesthetics and color,
round forms, babies, and tasks requiring interpersonal interaction.
See also Archetypes, Baby-Face Bias, Contour Bias, and Threat Detection.
1 See, for example, “Sex Differences in Infants’
Visual Interest in Toys” by Gerianne Alexander,
Teresa Wilcox, and Rebecca Woods, Archives
of Sexual Behavior, 2009, vol. 38, p. 427–433;
“Sex Differences in Interest in Infants Across
the Lifespan: A Biological Adaptation for
Parenting?” by Dario Maestripieri and Suzanne
Pelka, Human Nature, vol. 13(3), p. 327–344;
and “Sex Differences in Human Neonatal
Social Perception” by Jennifer Connellan,
Simon Baron-Cohen, Sally Wheelwright, et al.,
Infant Behavior & Development, 2000, vol.
23, p. 113–118.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Hunter-Nurturer Fixations 131
When vervets are presented with
human toys, female vervets prefer
stereotypically female toys and male
vervets prefer stereotypically male
toys. This suggests a biological basis
for gender-based play preferences in
primates — including humans.
The Pleo moves slowly and lacks
the predatory or angular features
that appeal to male children — better
to have made it a velociraptor. Its baby
face will appeal to female children, but
its reptilian semblance, rubber skin,
and rigid innards do not invite
nurturing — better to have made it a
soft, furry mammal. Despite its
technical sophistication, Pleo lacked
the basic elements necessary to
trigger hunter or nurturer fixations
in children, a likely factor in the
demise of its manufacturer, Ugobe.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Hunter-Nurturer Fixations** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Hunter-Nurturer Fixations để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Archetypes, Baby-Face Bias, Contour Bias, and Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
