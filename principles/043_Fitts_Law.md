---
name: "Fitts’ Law"
vi: "Định luật Fitts"
summary: "Fitts’ Law (Định luật Fitts): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Fitts’ Law (Định luật Fitts)

> **Tóm tắt cốt lõi (Summary)**: Fitts’ Law là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The time required to move to a target is a function of the
target size and distance to the target.
According to Fitts’ Law, the smaller and more distant a target, the longer it will
take to move to a resting position over the target. In addition, the faster the
required movement and the smaller the target, the greater the error rate due to
a speed-accuracy tradeoff. Fitts’ Law has implications for the design of controls,
control layouts, and any device that facilitates movement to a target.1
Fitts’ Law is applicable only for rapid, pointing movements, not for more
continuous movements, such as writing or drawing. It has been used to predict
efficiency of movement for assembly work performed under a microscope, as
well as movement of a foot to a car pedal. Pointing movements typically consist
of one large, quick movement toward a target (ballistic movement), followed
by fine-adjustment movements (homing movements) to a resting position over
(acquiring) the target. Homing movements are generally responsible for most of
the movement time and cause most errors.2
Designers can decrease errors and improve usability by understanding the
implications of Fitts’ Law. For example, when pointing to an object on a computer
screen, movement in the vertical or horizontal dimensions can be constrained,
which dramatically increases the speed with which objects can be accurately
acquired. This kind of constraint is commonly applied to controls such as scroll
bars, but less commonly to the edges of the screen, which also act as a barrier to
cursor movement; positioning a button along a screen edge or in a screen corner
significantly reduces the homing movements required, resulting in fewer errors
and faster acquisitions.
Consider Fitts’ Law when designing systems that involve pointing. Make sure
that controls are near or large, particularly when rapid movements are required
and accuracy is important. Likewise, make controls more distant and smaller
when they should not be frequently used, or when they will cause problems
if accidentally activated. Consider strategies that constrain movements when
possible to improve performance and reduce error.
See also Constraint, Errors, and Hick’s Law.
1 The seminal work on Fitts’ Law is “The
Information Capacity of the Human Motor
System in Controlling Amplitude of Movement”
by Paul M. Fitts, Journal of Experimental
Psychology, 1954, vol. 4, p. 381–191. The
Fitts’ law equation is MT = a + b log 2 (d/s + 1),
where MT = movement time to a target;
a = 0.230 sec; b = 0.166 sec; d = distance bet-
ween pointing device and target; and s = size
of the target. For example, assume the distance
between the center of a screen and an icon of
1” (3 cm) diameter is 6” (15 cm). The time to
acquire the icon would be MT = 0.230 sec
+ 0.166 sec (log 2 (6/1 + 1)) = 0.7 sec.
2 See “Human Performance Times in
Microscope Work” by Gary Langolf and Walton
M. Hancock, AIIE Transactions, 1975, vol.
7(2), p. 110–117; and “Application of Fitts’
Law to Foot-Pedal Design” by Colin G. Drury,
Human Factors, 1975, vol. 17(4), p. 368–373.
Fitts’ Law

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1/3" 3.94"
Fitts’ Law 99
Help
New Folder
View
Clean Up
Arrange
View Options ...
folder
folder
Steering
Wheel
Centerline
Brake
Accelerator 	Jeep Cherokee
Transmission
Hump
Jeep Cherokee Floorboard
Ford Taurus Floorboard
Distance from
steering wheel
centerline to right
edge of brake pedal
File 	Edit 	View Window 	Special 	Help
Empty Trash
Restart
Shut Down
Sleep
The Macintosh user
interface makes it easy to
move to a resting place over
menus. The top screen edge
stops the cursor, effectively
making the menus bigger by
giving them infinite height.
The time required to
acquire the closer, smaller
folder is the same as for
the distant, larger folder.
The Microsoft Windows user interface
presents pop-up menus when you
press the right mouse button. Since the
distance between the cursor position
and the pop-up menu is minimal,
menu items are quickly acquired.
In the 1990s, many cases of
unintended acceleration were reported
in Chrysler Jeep Cherokees. Brake
pedals are usually located to the right
of the steering wheel centerline, as in
the Ford Taurus. However, the Jeep
Cherokee’s large transmission hump
forced the pedal positions to the left.
This increased the distance between
foot and brake pedal, making the latter
more difficult to reach. This, combined
with a violation of convention, caused
Jeep Cherokee drivers to press the
accelerator when they intended to
press the brake pedal.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Fitts’ Law** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Fitts’ Law để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Constraint, Errors, and Hick’s Law
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
