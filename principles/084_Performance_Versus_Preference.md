---
name: "Performance Versus Preference"
vi: "Hiệu năng so với Sở thích cá nhân"
summary: "Performance Versus Preference (Hiệu năng so với Sở thích cá nhân): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Performance Versus Preference (Hiệu năng so với Sở thích cá nhân)

> **Tóm tắt cốt lõi (Summary)**: Performance Versus Preference là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The designs that help people perform optimally are often not
the same as the designs that people find most desirable.
Designers and managers often confuse the business maxim “the customer is
always right” with “the user is always is right.” This is a dangerous confusion, since
what helps people perform well and what people like is often not the same thing.
For example, the Dvorak keyboard is estimated to improve typing efficiency by
more than 30 percent, but has failed to rise in popularity because people prefer the
more familiar QWERTY keyboard. If you asked people if they would like to be able
to type 30 percent faster with fewer errors, most would answer in the affirmative.
Despite this, more than 50 years have passed since the introduction of the Dvorak
keyboard, and it is still more of a novelty item than a practical alternative.1
This underscores an important lesson for designers: the reasons people prefer
one design to another is a combination of many factors, and may have nothing
to do with performance. Is the design pleasing to look at? Does it compete with
long-standing designs or standards of use? Does it contribute to the well-being or
self-esteem of the user? These are all factors that must be carefully balanced in the
development of the design requirements. If a superbly performing design is never
bought or used because people (for whatever reason) do not prefer it to alternatives,
the performance benefits are moot. Conversely, if a well-liked design does not help
people perform at the level required, the preference benefits are moot.
The best way to correctly balance performance and preference in design is to
accurately determine the importance of performance versus preference. While
surveys, interviews, and focus groups try to find out what people want or like,
they are unreliable indicators of what people will actually do, especially for new
or unfamiliar designs. Additionally, people are poor at discriminating between
features they like, and features that actually enhance their performance; they
commonly prefer designs that perform less well than available alternatives, and
incorrectly believe that those designs helped them achieve the best performance.2
The best method of obtaining accurate performance and preference requirements
is to observe people interacting with the design (or a similar design) in real
contexts. When this is not feasible, test using structured tasks that approximate
key aspects of the way the design will be used. It is important to obtain preference
information in context while the task is being performed, and not afterward. Do not
rely on reports of what people say they have done, will do, or are planning to do in
the future regarding the use of a design; such reports are unreliable.
See also Aesthetic-Usability Effect, Control, Development Cycle,
Flexibility-Usability Tradeoff, and Hierarchy of Needs.

1 See, for example, “Performance Versus
Preference” by Robert W. Bailey, Proceedings
of the Human Factors and Ergonomics Society
37th Annual Meeting, 1993, p. 282–286.
Note that the widely accepted belief that
the Dvorak layout is superior to QWERTY in
terms of typing performance is not without its
skeptics. Critics charge that early tests favoring
the Dvorak layout were biased and poorly
constructed, while modern comparisons show
little, if any, performance difference. See, for
example, “The Fable of the Keys” by Stan
Liebowitz and Stephen Margolis, in Famous
Fables of Economics by Dan Spulber (ed.),
Blackwell Publishers, 2002; Journal of Law
and Economics, vol. 30(1), p. 1–26, April
1990. Anecdotally, the world’s fastest typist
when The Guinness Book of World Records
included the category, Barbara Blackburn,
died in 2008—she used a Dvorak.
2 See, for example, “Measuring Usability:
Preference vs. Performance” by Jakob Nielsen
and Jonathan Levy, Communications of the
ACM, 1994, vol. 37(4), p. 66–75.
Performance Versus Preference

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

1
R 	T 	Y	Q 	W 	E 	U 	I 	O 	P
A 	S 	D 	F 	G 	H 	J 	K 	L
Z 	X 	C 	V 	B 	N 	M
!
/
?
,
< .
>
2
@ 3
# 4
$ 5
% 6
^ 7
& 8
* 9
( 0
) –
— =
+
\|
]
}
'"
[
{
;:
1
P 	Y 	F 	G 	C 	R 	L
A 	O 	E 	U 	I 	D 	H 	T 	N 	S
Q 	J 	K 	X 	B 	M 	W 	V 	Z
!
/
?
,
< .
>
2
@ 3
# 4
$ 5
% 6
^ 7
& 8
* 9
( 0
)
–
—
=
+ \|
]
}
'"
[
{
;
:
The QWERTY layout was designed to
prevent the jamming of mechanical
arms on early typewriters. The Dvorak
layout, by contrast, was designed to
maximize typing efficiency: it grouped
keys based on frequency of use, and
positioned keys to promote alternating
keystrokes between hands, among
other refinements. The result is a
30 percent improvement in typing
efficiency, and claim to most of
the world records for speed typing.
Despite the clear advantages of the
Dvorak design, QWERTY enjoys the
following of generations of people
trained on the layout, which in turn
drives manufacturers to continue
perpetuating the standard. Dvorak
wins on performance, but QWERTY
wins on preference.
Performance Versus Preference 181
QWERTY Keyboard
shift
return
return
Dvorak Keyboard
shift

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Performance Versus Preference** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Performance Versus Preference để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Aesthetic-Usability Effect, Control, Development Cycle,
Flexibility-Usability Tradeoff, and Hierarchy of Needs
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
