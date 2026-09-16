---
name: "Mapping"
vi: "Ánh xạ điều khiển (Mapping)"
summary: "Mapping (Ánh xạ điều khiển (Mapping)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - usability
---

# Universal Design Principle: Mapping (Ánh xạ điều khiển (Mapping))

> **Tóm tắt cốt lõi (Summary)**: Mapping là một nguyên lý thiết kế then chốt thuộc nhóm **perception, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Mapping
A relationship between controls and their movements or
effects. Good mapping between controls and their effects
results in greater ease of use.1
Turn a wheel, flip a switch, or push a button, and you expect some kind of
effect. When the effect corresponds to expectation, the mapping is considered
to be good or natural. When the effect does not correspond to expectation, the
mapping is considered to be poor. For example, an electric window control on a
car door can be oriented so that raising the control switch corresponds to raising
the window, and lowering the control switch lowers the window. The relationship
between the control and raising or lowering the window is obvious. Compare this
to an orientation of the control switch on the surface of an armrest, such that the
control motion is forward and backward. The relationship between the control and
the raising and lowering of the window is no longer obvious; does pushing the
control switch forward correspond to raising or lowering the window?2
Good mapping is primarily a function of similarity of layout, behavior, or meaning.
When the layout of stovetop controls corresponds to the layout of burners, this
is similarity of layout; when turning a steering wheel left turns the car left, this is
similarity of behavior; when an emergency shut-off button is colored red, this is
similarity of meaning (e.g., most people associate red with stop). In each case,
similarity makes the control-effect relationship predictable, and therefore easy to use.3
Position controls so that their locations and behaviors correspond to the layout and
behavior of the device. Simple control-effect relationships work best. Avoid using
a single control for multiple functions whenever possible; it is difficult to achieve
good mappings for a one control-multiple effect relationship. In cases where this
is not possible, use visually distinct modes (e.g., different colors) to indicate active
functions. Be careful when relying on conventions to attach meaning to controls,
as different population groups may interpret the conventions differently (e.g., in
England, flipping a lightswitch up turns it off and flipping it down turns it on).
See also Affordance, Interference Effects, Nudge, Proximity, and Visibility.

1 Also known as control-display relationship and
stimulus-response compatibility.
2 The seminal work on mapping is The Design
of Everyday Things by Donald Norman,
Doubleday, 1990.
3 For a review of these kinds of issues, see
Spatial Schemas and Abstract Thought by
Merideth Gattis (ed.), MIT Press, 2001.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Mapping 153
Lean
backward
to travel
backward
Lean
forward
to travel
forward
The relationship between stovetop
controls and burners is ambiguous
when the controls are horizontally
oriented and equally spaced
(poor mapping). The relationship
becomes clearer when the controls
are grouped with the burners, but
the horizontal orientation still confuses
which control goes with which burner
(poor, but improved mapping). When
the layout of the controls corresponds
to the layout of the burners, the
control-burner relationships are clear
(good mapping).
The relationship between the
window control and the raising
and lowering of the window is
obvious when it is mounted on
the wall of the door (good mapping),
but ambiguous when mounted
on the surface of the armrest
(poor mapping).
The Segway Human Transporter
makes excellent use of mapping.
Lean forward to go forward, and
lean backward to go backward.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Mapping** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Mapping để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Interference Effects, Nudge, Proximity, and Visibility
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
