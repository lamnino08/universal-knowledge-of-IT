---
name: "Most Average Facial Appearance Effect"
vi: "Hiệu ứng khuôn mặt trung bình"
summary: "Most Average Facial Appearance Effect (Hiệu ứng khuôn mặt trung bình): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Most Average Facial Appearance Effect (Hiệu ứng khuôn mặt trung bình)

> **Tóm tắt cốt lõi (Summary)**: Most Average Facial Appearance Effect là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A tendency to prefer faces in which the eyes, nose, lips,
and other features are close to the average of a population.1
People find faces that approximate their population average more attractive than
faces that deviate from their population average. In this context, population refers
to the group in which a person lives or was raised, and average refers to the
arithmetic mean of the form, size, and position of the facial features. For example,
when pictures of many faces within a population are combined (averaged) to
form a single composite image, the composite image is similar to the facial
configurations of professional models in that population.2
The most average facial appearance effect is likely the result of some combination
of evolution, cognitive prototypes, and symmetry. Evolution by natural selection
tends to select out extremes from a population over time. Therefore, it is
possible that a preference for averageness has evolved as an indicator of general
fitness. Cognitive prototypes are mental representations that are formed through
experience. As people see the faces of other people, their mental representation
of what a face is may be updated through a process similar to compositing. If
this is the case, average faces pattern-match easily with cognitive prototypes, and
contribute to a preference. Finally, average faces are symmetrical, and symmetry
has long been viewed as an indicator of health and fitness. Asymmetric members
of all species tend to have fewer offspring and live shorter lives—generally the
asymmetry is the result of disease, malnutrition, or bad genes.3
The evolution of racial preferences among isolated ethnic groups demonstrates
the influence of the most average facial appearance effect. Isolated groups form
cognitive prototypes based on the faces within their population. When two of these
groups first encounter one another, they invariably regard members of the unfamiliar
group as strange and less attractive. The facial appearance of unfamiliar groups is
perceived as less attractive because it is further from the average facial appearance
of the familiar group. As the differences become more familiar, however, cognitive
prototypes are updated and the definition of facial beauty changes.
The most average facial appearance for a population is an accurate benchmark
of beauty for that population. There are other elements that contribute to
attractiveness (e.g., smile versus scowl), but faces that are not average will
not be perceived as attractive. Use composite images of faces created from
randomly sampled faces of target populations to indicate local perceptions of
beauty. Consider the use of digital compositing and morphing software to develop
attractive faces from common faces for advertising and marketing campaigns,
especially when real models are unavailable or budgetary resources are limited.
See also Attractiveness Bias, Baby-Face Bias, Mental Model, Normal Distribution,
and Symmetry.

1 Also referred to as MAFA effect.
2 The seminal work on the most average facial
appearance effect is “Attractive Faces are Only
Average” by Judith H. Langlois and Lori A.
Roggman, Psychological Science, 1990, vol. 1,
p. 115–121.
3 See, for example, “Developmental Stability,
Disease, and Medicine” by Randy Thornhill
and Anders P. Møller, Biological Reviews,
1997, vol. 72, p. 497–548.
Most Average Facial Appearance Effect

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The most average facial
appearance for a population is
also the most attractive. In this
population of four men and
four women, two generations
of composites were created to
demonstrate the effect. Unique
and idiosyncratic facial features
are minimized and overall
symmetry is improved.
Most Average Facial Appearance Effect 165
Source
1st Generation Composite
2nd Generation Composite—MAFA
1st Generation Composite
Source

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Most Average Facial Appearance Effect** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Most Average Facial Appearance Effect để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Attractiveness Bias, Baby-Face Bias, Mental Model, Normal Distribution,
and Symmetry
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
