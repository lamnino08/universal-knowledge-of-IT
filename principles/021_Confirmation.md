---
name: "Confirmation"
vi: "Xác nhận hành động (Confirmation)"
summary: "Confirmation (Xác nhận hành động (Confirmation)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
---

# Universal Design Principle: Confirmation (Xác nhận hành động (Confirmation))

> **Tóm tắt cốt lõi (Summary)**: Confirmation là một nguyên lý thiết kế then chốt thuộc nhóm **usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A technique for preventing unintended actions by requiring
verification of the actions before they are performed.1
Confirmation is a technique used for critical actions, inputs, or commands. It
provides a means for verifying that an action or input is intentional and correct
before it is performed. Confirmations are primarily used to prevent a class of errors
called slips, which are unintended actions. Confirmations slow task performance,
and should be reserved for use with critical or irreversible operations only. When
the consequences of an action are not serious, or when actions are completely and
easily reversible, confirmations are not needed. There are two basic confirmation
techniques: dialog and two-step operation.2
Confirmation using a dialog involves establishing a verbal interaction with the
person using the system. It is most commonly represented as a dialog box on a
software display (e.g., “Are you sure you want to delete all files?”). In this method,
dialog boxes directly ask the user if the action was intended and if they would like
to proceed. Confirmations should be used sparingly, or people will become frus-
trated at the frequent interruption and then learn to ignore them. Dialog messages
should be concise but detailed enough to accurately convey the implications of
the action. The message should end with one question that is structured to be
answered Yes or No, or with an action verb that conveys the action to be performed
(the use of OK and Cancel should be avoided for confirmations). For less critical
confirmations that act more as reminders, an option to disable the confirmation
should be provided.
Confirmation using a two-step operation involves a preliminary step that must occur
prior to the actual command or input. This is most often used with hardware
controls, and is often referred to as an arm/fire operation—first you arm the
component, and then you fire (execute) it. For example, a switch cover might have
to be lifted in order to activate a switch, two people might have to turn two unique
keys in order to launch a nuclear weapon, or a control handle in a spacecraft might
have to be rotated and then pushed down in order to be activated. The purpose
of the two-step operation is to prevent accidental activation of a critical control.
If the operation works only when the two-step sequence has been completed,
it is unlikely that the operation will occur accidentally. Two-step operations are
commonly used for critical operations in aircraft, nuclear power plants, and other
environments involving dangerous operations.
Use confirmations to minimize errors in the performance of critical or irreversible
operations. Avoid overusing confirmations to ensure that they are unexpected
and uncommon; otherwise, they may be ignored. Use a two-step operation for
hardware confirmations, and a dialog box for software confirmations. Permit less
critical confirmations to be disabled after an initial confirmation.
See also Constraint, Errors, Forgiveness, and Garbage In–Garbage Out.

1 Also known as verification principle and
forcing function.
2 See, for example, The Design of Everyday
Things by Donald Norman, Doubleday, 1990;
and To Err Is Human: Building a Safer Health
System edited by Linda T. Kohn, Janet M.
Corrigan, and Molla S. Donaldson, National
Academy Press, 2000.
Confirmation

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Confirmation 55
Launch Rocket
Send Now 	Categories
Road Runner
info@stuffcreators.com
You have not entered a subject. It is recommended
that all messages have subjects. Would you like to
send the message anyway?
Don’t show this message again
Cancel 	Send
From:
To:
Cc:
Subject:
Attac
Mo
untitled
Register
Enter a UserID:
Enter a Password:
Re-Enter Your Password:
Submit 	Cancel
WARNING
DO NOT REMOVE
	THIS LOCK
ANGER
EQUIPMENT
	LOCKED OUT
THIS TAG AND LOCK TO
	BE REMOVED
	ONLY BY PERSON LISTED BELOW
	NAME
DATE
Common examples of confirmation
strategies include: typing in a password
twice to confirm spelling; confirming
the intent of an action by clicking the
action button (Send) with an option to
disable future confirmations; having
to remove a lock to open a valve; and
having to turn two unique keys to
complete a launch circuit.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Confirmation** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Confirmation để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Constraint, Errors, Forgiveness, and Garbage In–Garbage Out
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
