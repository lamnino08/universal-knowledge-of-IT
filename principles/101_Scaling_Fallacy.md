---
name: "Scaling Fallacy"
vi: "Ngụy biện về quy mô (Scaling Fallacy)"
summary: "Scaling Fallacy (Ngụy biện về quy mô (Scaling Fallacy)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Scaling Fallacy (Ngụy biện về quy mô (Scaling Fallacy))

> **Tóm tắt cốt lõi (Summary)**: Scaling Fallacy là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

1 Also known as cube law and law of sizes.
2 The seminal work on scaling is Dialogues
Concerning Two New Sciences by Galileo
Galilei, Prometheus Books [reprint], 1991.
3 “Design Flaw Seen as Failure Cause in Trident
2 Tests” by Andrew Rosenthal, New York
Times, August 17, 1989, p. 1.

Scaling Fallacy
A tendency to assume that a system that works at one
scale will also work at a smaller or larger scale.1
Much is made of the relative strength of small insects as compared to that
of humans. For example, a leafcutter ant can carry about 50 times its weight;
whereas an average human can only carry about half its weight. The standard
reasoning goes that an ant scaled to the size of a human would retain this
strength-weight advantage, giving a 200-pound ant the ability to lift 10,000 pounds.
In actuality, however, an ant scaled to this size would only be able to lift about
50 pounds, assuming it could move at all. The effect of gravity at small scales is
miniscule, but the effect increases dramatically with the size of an object. This
underscores the basic lesson of the scaling fallacy—systems act differently at
different scales. There are two basic kinds of scaling assumptions to avoid when
growing or shrinking a design: load assumptions, and interaction assumptions.2
Load assumptions occur when designers scale a design by some factor, and
assume that the working stresses on the design scale by that same factor. For
example, initial designs of the Trident 2 missile, designed to be launched from
submarines, underestimated the effects of water pressure and turbulence during
launch. The anticipated estimates for pressure and turbulence were based largely
on the Trident 1 missile, which was much shorter and roughly half the weight
of the Trident 2. When the specifications for the Trident 1 were scaled to meet
the specifications for the Trident 2, the working stresses on the missile did not
scale by the same factor as its physical specification. The result was multiple
catastrophic failures in early tests, and a major redesign of the missile.3
Interaction assumptions occur when designers scale a design, and assume that
the way people and other systems interact with the design will be the same at
other levels of scale. For example, the design of very tall buildings involves many
possible interactions that do not exist for buildings of lesser size—problems of
evacuation in the case of fire, people seeking to commit suicide or base-jump
off of the roof, symbolic target for terrorist attacks, to name a few. These kinds
of interaction effects are usually an indirect consequence of the design, and
therefore can be difficult to anticipate and manage.
The best way to avoid the scaling fallacy is to be aware of the tendency to
make scaling assumptions. Therefore, raise awareness of load and interaction
assumptions in the design process. Verify load assumptions through the use of
careful calculations, systematic testing, and appropriate factors of safety. Minimize
incorrect interaction assumptions through careful research of analogous designs,
and monitoring of how the design is used once implemented.
See also Factor of Safety, Feedback Loop, Modularity, and Structural Forms.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1
10-1
10-2
10-3
10-4
Scaling Fallacy 215
Meters
The scaling fallacy is nowhere
more apparent than with flight. For
example, at very small and very large
scales, flapping to fly is not a viable
strategy. At very small scales, wings
are too small to effectively displace
air molecules. At very large scales,
the effects of gravity are too great for
flapping to work—a painful lesson
learned by many early pioneers
of human flight. The lesson is that
designs can be effective at one scale,
and completely ineffective at another.
The images from small to large:
aeroplankton simply float about in
air; baby spiders use tiny web sails
to parachute; insects flap to fly; birds
flap to fly; humans flap but do not fly.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Scaling Fallacy** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Scaling Fallacy để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Factor of Safety, Feedback Loop, Modularity, and Structural Forms
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
