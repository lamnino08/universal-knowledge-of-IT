---
name: "Forgiveness"
vi: "Tính khoan dung (Forgiveness)"
summary: "Forgiveness (Tính khoan dung (Forgiveness)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - learning
---

# Universal Design Principle: Forgiveness (Tính khoan dung (Forgiveness))

> **Tóm tắt cốt lõi (Summary)**: Forgiveness là một nguyên lý thiết kế then chốt thuộc nhóm **usability, learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Forgiveness
Designs should help people avoid errors and minimize the
negative consequences of errors when they do occur.
Human error is inevitable, but it need not be catastrophic. Forgiveness in design
helps prevent errors before they occur, and minimizes the negative consequences
of errors when they do occur. Forgiving designs provide a sense of security and
stability, which in turn, fosters a willingness to learn, explore, and use the design.
Common strategies for incorporating forgiveness in designs include:
Good Affordances—physical characteristics of the design that influence its
correct use (e.g., uniquely shaped plug that can only be inserted into the
appropriate receptacle).
Reversibility of Actions— one or more actions can be reversed if an error occurs or
the intent of the person changes (e.g., undo function in software).
Safety Nets—device or process that minimizes the negative consequences of a
catastrophic error or failure (e.g., pilot ejection seat in aircraft).
Confirmation—verification of intent that is required before critical actions are
allowed (e.g., lock that must be opened before equipment can be activated).
Warnings—signs, prompts, or alarms used to warn of imminent danger (e.g., road
signs warning of a sharp turn ahead).
Help —information that assists in basic operations, troubleshooting, and error
recovery (e.g., documentation or help line).
The preferred methods of achieving forgiveness in a design are affordances,
reversibility of actions, and safety nets. Designs that effectively use these strategies
require minimal confirmations, warnings, and help—i.e., if the affordances are
good, help is less necessary; if actions are reversible, confirmations are less
necessary; if safety nets are strong, warnings are less necessary. When using
confirmations, warnings, and help systems, avoid cryptic messages or icons.
Ensure that messages clearly state the risk or problem, and also what actions can
or should be taken. Keep in mind that too many confirmations or warnings impede
the flow of interaction and increase the likelihood that the confirmation or warning
will be ignored.
Create forgiving designs by using good affordances, reversibility of actions, and
safety nets. If this is not possible, be sure to include confirmations, warnings, and
a good help system. Be aware that the amount of help necessary to successfully
interact with a design is inversely proportional to the quality of the design—if a lot
of help is required, the design is poor.
See also Affordance, Confirmation, Errors, Factor of Safety, and Nudge.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

25mph
Forgiveness 105
WARNING
	DO NOT REMOVE
	THIS LOCK
ANGER
EQUIPMENT
	LOCKED OUT
THIS TAG AND LOCK TO BE REMOVED
ONLY BY PERSON
 LISTED BELOW
NAME
DATE
History 	Actions 	Tool Presets
pods.jpg
Open
Image Size
Brightness/Contrast
CMYK Color
Image Size
Select Canvas
Rotate
Stroke
New Layer
New Layer
Select Canvas
Fill
Deselect
Select Canvas
Cut Pixels
Paste
Road signs make roads more
forgiving by warning drivers of
impending hazards.
Locking and tagging equipment is
a common confirmation strategy to
ensure that people do not accidentally
engage systems under repair.
The good affordance of this plug
prevents it from being inserted into
the socket improperly.
The Adobe Photoshop History palette
enables users to flexibly undo and
redo their previous actions.
In case of a catastrophic failure, the
ballistic recovery system acts as a
safety net, enabling the pilot and craft
to return safely to earth.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Forgiveness** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Forgiveness để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Affordance, Confirmation, Errors, Factor of Safety, and Nudge
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
