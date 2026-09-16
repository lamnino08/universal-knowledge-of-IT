---
name: "Mental Model"
vi: "Mô hình tâm trí (Mental Model)"
summary: "Mental Model (Mô hình tâm trí (Mental Model)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - usability
---

# Universal Design Principle: Mental Model (Mô hình tâm trí (Mental Model))

> **Tóm tắt cốt lõi (Summary)**: Mental Model là một nguyên lý thiết kế then chốt thuộc nhóm **learning, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Mental Model
People understand and interact with systems and
environments based on mental representations developed
from experience.
Mental models are representations of systems and environments derived from
experience. People understand and interact with systems and environments by
comparing the outcomes of their mental models with the real-world systems and
environments. When the outcomes correspond, a mental model is accurate and
complete. When the outcomes do not correspond, the mental model is inaccurate
or incomplete. With regards to design, there are two basic types of mental models:
mental models of how systems work (system models) and mental models of how
people interact with systems (interaction models).1
Designers generally have very complete and accurate system models, but often
have weak interaction models—i.e., they know much about how a system works,
but little about how people will interact with the system. Conversely, users of a
design tend to have sparse and inaccurate system models, but through use and
experience commonly attain interaction models that are more complete and
accurate than those of designers. Optimal design results only when designers
have an accurate and complete system model, attain an accurate and complete
interaction model, and then design a system interface that reflects an efficient
merging of both models.2
Designers can obtain accurate and complete interaction models through personal
use of the system, laboratory testing (e.g., focus groups and usability testing),
and direct observation of people interacting with the system, or similar systems.
Use of the system by the designer will reveal obvious design problems, but will
fail to reveal the problems of interaction that emerge when people are unfamiliar
with the system. Laboratory testing is useful for evaluating designs in a controlled
environment, but must be conducted with care, as the artificial context and
expectation effects can compromise the validity of the results. Direct observation
in the target environment is the preferred method for acquiring accurate
information about how people interact with systems, but is costly and impractical
for designs that are not yet publicly available.
Design with people’s interaction models in mind. If there is a standard mental
model for how something works, try to design leveraging that model. When this is
not possible, (e.g., the system is new and novel), create an interaction experience
that draws from common mental models as much as possible, such as the
desktop metaphor for computers. However, do not contrive design just to leverage
a familiar model—it is better to have people learn a new model that is clear and
consistent, than to use a familiar model that does not fit. Use the systems that you
design, and employ laboratory testing and field observation in order to develop
accurate and complete interaction models. Above all, watch people use the design
and take note of how they use it.
See also Affordance, Expectation Effects, Mapping, and Mimicry.

1 The seminal works on mental models are
The Nature of Explanation by Kenneth Craik,
Cambridge University Press, 1943; and Mental
Models: Towards a Cognitive Science of
Language, Inference, and Consciousness by
Philip N. Johnson-Laird, Cambridge University
Press, 1983. For a design perspective, see
“Surrogates and Mappings: Two Kinds of
Conceptual Models for Interactive Devices” by
Richard M. Young, and “Some Observations
on Mental Models” by Donald Norman, both in
Mental Models by D. Gentner and A. Stevens
(Eds.), Lawrence Erlbaum Associates, 1983.
2 Note that an efficient merging does not simply
mean revealing the system model. It may
mean concealing the system model from
users, revealing the system model to users,
or a combination therein.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Despite the measurable safety benefits
of antilock brakes in controlled tests
with trained drivers, research by the
Highway Loss Data Institute indicates
that antilock brakes have not reduced
the frequency or cost of accidents in
real-world driving situations.
The likely cause is that people are not
using antilock brakes properly—or
rather; antilock brakes are not
designed properly. The interaction
model for antilock brakes differs
radically from the interaction model
for conventional brakes.
This suggests that designers gave
little consideration to the interaction
models of the target audience in the
design process.
Mental Model 155
Interaction Model for Conventional Brakes
On slick surfaces...
• depress the brake pedal smoothly
• pump brakes to prevent brakes from locking up
• do not steer while braking, except to counter-steer
• noise and vibration are signs that something is wrong
Interaction Model for ABS Brakes
On slick surfaces...
• depress the brake pedal fast and hard
• do not pump brakes
• steer while braking
• noise and vibration are signs that the system is operating properly
INCORRECT INTERACTION
slamming brakes/steering while braking
Car will take a longer time to stop and will not make the turn
CORRECT INTERACTION
slamming brakes/steering while braking
Car will properly stop and make the turn
INCORRECT INTERACTION
pumping brakes
Car will take a longer time to stop and will not make the turn
CORRECT INTERACTION
pumping brakes
Car will take a shorter time to stop and may make the turn
wet, slick surface 	wet, slick surface 	wet, slick surface 	wet, slick surface
wet, slick surface 	wet, slick surface 	wet, slick surface 	wet, slick surface

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Mental Model** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Mental Model để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Expectation Effects, Mapping, and Mimicry
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
