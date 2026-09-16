---
name: "Contour Bias"
vi: "Thiên kiến đường cong"
summary: "Contour Bias (Thiên kiến đường cong): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - appeal
---

# Universal Design Principle: Contour Bias (Thiên kiến đường cong)

> **Tóm tắt cốt lõi (Summary)**: Contour Bias là một nguyên lý thiết kế then chốt thuộc nhóm **perception, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Contour Bias
A tendency to favor objects with contours over objects
with sharp angles or points.
When presented with objects that possess sharp angles or pointed features, a
region of the human brain involved in fear processing, the amygdala, is activated.
Likely a subconscious mechanism that evolved to detect potential threats, this
fear response suggests that angular features influence the way in which objects
are affectively and aesthetically perceived. Indeed, in experiments where subjects
were presented with otherwise similar angled versus contoured objects (e.g.,
round-faced watches versus square-faced watches), subjects strongly preferred
the more rounded, contoured objects. In some of these experiments, brain activity
was observed using functional magnetic resonance imaging (fMRI) as subjects
indicated their preference. The degree of amygdala activation was proportional
to the degree of angularity or sharpness of the object presented, and inversely
related to object preference. These effects were observed in both male and
female subjects, and suggest an innately rooted contour bias in humans.1
The picture is more complex, however, than to simply infer that all designs should
be made round to increase their appeal. Objects used in the experiments were
emotionally neutral. For example, a baby doll was not used for a contour object
as it carries with it a set of positive emotional associations and biases, and a
knife was not used for an angular object as it carries with it a set of negative
emotional associations and biases. It is clear that absent these competing biases
and associations, the contour bias is a relevant influencer of overall perception.
The degree to which the bias influences perception when competing biases
(e.g., baby-face bias) or semantically relevant perceptions (e.g., criminals use
knives) are at play is not yet clear. Additionally, objects with pointed features
elicited stronger activations in regions of the brain related to associative
processing, meaning that although the angular objects were less liked, they
elicited a deeper level of processing than did the contoured objects — they were,
in effect, more interesting and thought-provoking to look at. This seems consistent
with the kind of innate response one would expect from potential threats and
suggests a tradeoff between angular and contoured features: Angular objects are
more effective at attracting attention and engaging thought; contoured objects are
more effective at making a positive emotional and aesthetic impression.
Consider the contour bias in all aspects of design, but especially with regard to
objects and environments that are emotionally neutral. Use angular and pointy
features to attract attention and provoke thought. Use contoured features to make
a positive first impression. Generally, the degree of angularity corresponds with the
strength of amygdala activation, so ensure that the angularity of design elements
aligns with the design objectives.
See also Archetypes, Baby-Face Bias, Freeze-Flight-Fight-Forfeit,
Hunter-Nurturer Fixations, and Threat Detection.
1 The seminal work on the contour bias is
“Humans Prefer Curved Visual Objects” by
Moshe Bar and Maital Neta, Psychological
Science, 2006, vol. 17. See also “Visual
Elements of Subjective Preference Modulate
Amygdala Activation” by Moshe Bar and
Maital Neta, Neuropsychologia, 2007, vol. 45.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Contour Bias 63
From top left to bottom right, the
Alessi il Conico, 9093, 9091, and
Mami kettles arranged from most
angular to most contoured. At the
extremes of this continuum, the
il Conico will be most effective at
grabbing attention, and the Mami will
be most liked generally. The 9093
and 9091 incorporate both angular
and contoured features, balancing
attention-getting with likeability.
Historically, the il Conico and 9093 are
Alessi’s best-selling kettles.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Contour Bias** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Contour Bias để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Archetypes, Baby-Face Bias, Freeze-Flight-Fight-Forfeit,
Hunter-Nurturer Fixations, and Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
