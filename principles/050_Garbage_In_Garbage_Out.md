---
name: "Garbage In–Garbage Out"
vi: "Dữ liệu vào rác - Kết quả ra rác (GIGO)"
summary: "Garbage In–Garbage Out (Dữ liệu vào rác - Kết quả ra rác (GIGO)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - decision
---

# Universal Design Principle: Garbage In–Garbage Out (Dữ liệu vào rác - Kết quả ra rác (GIGO))

> **Tóm tắt cốt lõi (Summary)**: Garbage In–Garbage Out là một nguyên lý thiết kế then chốt thuộc nhóm **learning, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Garbage In–Garbage Out
The quality of system output is dependent on the quality
of system input.1
The garbage in–garbage out principle is based on the observation that good inputs
generally result in good outputs, and bad inputs, barring design intervention,
generally result in bad outputs. The rule has been generalized over time to apply
to all systems, and is commonly invoked in domains such as business, education,
nutrition, and engineering, to name a few. The “garbage in” metaphor refers to
one of two kinds of input problems: problems of type and problems of quality.2
Problems of type occur when the incorrect type of input is fed into a system, such
as entering a phone number into a credit card number field. Problems of type
are serious because the input provided could be radically different from the input
expected. This can be advantageous in that problems of type are relatively easy
to detect, but problematic in that they represent the maximum form of garbage
if undetected. Problems of type are generally caused by a class of errors called
mistakes—incorrect actions caused by conscious actions. The primary strategies
for minimizing problems of type are affordances and constraints. These strategies
structure input and minimize the frequency and magnitude of garbage input.
Problems of quality occur when the correct type of input is fed into a system, but
with defects, such as entering a phone number into a phone number field but
entering the wrong number. Depending on the frequency and severity of these
defects, problems of quality may or may not be serious. Mistyping one letter
in a name may have minor consequences (e.g., search item not found); trying
to request a download of fifty records but typing five thousand might lock up
the system. Problems of quality are generally caused by a class of errors called
slips—incorrect actions caused by unconscious, accidental actions. The primary
strategies for minimizing problems of quality are previews and confirmations.
These strategies allow the consequences of actions to be reviewed and verified
prior to input.
The best way to avoid garbage out is to prevent garbage in. Use affordances and
constraints to minimize problems of type. Use previews and confirmations to
minimize problems of quality. When input integrity is critical, use validation tests
to check integrity prior to input, and consider confirmation steps that require the
independent verification of multiple people. Consider mechanisms to automatically
flag and, in some cases, autocorrect bad input (e.g., automatic spelling correction
in word processors).
See also Errors, Feedback Loop, and Signal-to-Noise Ratio.
1 Also known as GIGO.
2 While the garbage in–garbage out concept
dates back to Charles Babbage (1864),
or earlier, the term is attributed to George
Fuechsel, a programming instructor who
used it as a teaching device in the late
1950s. It should be noted that Fuechsel
used the principle to emphasize that
“garbage out” is not the inevitable result
of “garbage in,” but rather a condition that
should be addressed through design.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Garbage In–Garbage Out 113
Order Form: Billing and Shipping Information 	page 2 of 2
Shipping Address: 	Billing Address:
Name 	Name
Street Address 	Street Address
Street Address 	Street Address
City, State and Zip Code 	City, State and Zip Code
Credit Card Information:
Name on Credit Card 	Type of Credit Card 	Credit Card Number 	Exp. Date
Shipping Method: 	Date to Ship:
continue
Your order will not be placed until you
review the information you entered and
click the “submit order” button.
March 21, 2003
1 dozen
chocolate chip cookies
Ship to:
Randy Williams
101 Main Street
Houston, TX 90990
Ship on:
March 30, 2003
Bill to:
Kristen Johnson
211 Elm Blvd.
Columbus, OH 44356
VISA: **** **** **** 3041
Exp. Date 5/2006
Name on Card: Kristen J. Johnson
make changes 	submit order
Unconstrained fields
increase the probability of
garbage input.
Allow users to automate
input by accessing stored
information.
Constrain input when a
specific amount of
information is required.
Constrain input using
menus of options.
Allow users to preview
information before they
complete transactions.
Billing Address
click here if Billing Address is the same as Shipping Address
Order Form: Billing and Shipping Information 	page 2 of 2
click here to use the information saved with your account
Shipping Address:
First Name 	Last Name 	First Name 	Last Name
Street Address 	Street Address
City 	State 	Zip Code 	City 	State 	Zip Code
Credit Card Information:
Name on Card 	Type of Card 	Month 	Year
Credit Card Number 	Expiration Date
Shipping Method: 	Date to Ship:
Standard Shipping $7.00 	Month 	Day 	Year
continue
Original Form
Redesigned Form
These two different designs of the
same order form illustrate how
designers can influence the amount
of garbage entered into a system.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Garbage In–Garbage Out** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Garbage In–Garbage Out để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Errors, Feedback Loop, and Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
