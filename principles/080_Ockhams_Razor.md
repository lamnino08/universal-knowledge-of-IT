---
name: "Ockham’s Razor"
vi: "Dao cạo Ockham"
summary: "Ockham’s Razor (Dao cạo Ockham): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Ockham’s Razor (Dao cạo Ockham)

> **Tóm tắt cốt lõi (Summary)**: Ockham’s Razor là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Ockham’s Razor
Given a choice between functionally equivalent designs,
the simplest design should be selected.1
Ockham’s razor asserts that simplicity is preferred to complexity in design. Many
variations of the principle exist, each adapted to address the particulars of a field
or domain of knowledge. A few examples include:
• “Entities should not be multiplied without necessity.”—William of Ockham
• “That is better and more valuable which requires fewer, other
circumstances being equal.”—Robert Grosseteste
• “Nature operates in the shortest way possible.”—Aristotle
• “We are to admit no more causes of natural things than such as are both
true and sufficient to explain their appearances.”—Isaac Newton
• “Everything should be made as simple as possible, but not simpler.”
—Albert Einstein
Implicit in Ockham’s razor is the idea that unnecessary elements decrease a
design’s efficiency, and increase the probability of unanticipated consequences.
Unnecessary weight, whether physical, visual, or cognitive, degrades performance.
Unnecessary design elements have the potential to fail or create problems.
There is also an aesthetic appeal to the principle, which likens the “cutting”
of unnecessary elements from a design to the removal of impurities from a
solution—the design is a cleaner, purer result.
Use Ockham’s razor to evaluate and select among multiple, functionally equivalent
designs. Functional equivalence here refers to comparable performance of a design
on common measures. For example, given two functionally equivalent displays—
equal in information content and readability—select the display with the fewest
visual elements. Evaluate each element within the selected design and remove as
many as possible without compromising function. Finally, minimize the expression
of the remaining elements as much as possible without compromising function.2
See also Form Follows Function, Horror Vacui, Mapping, and Signal-to-Noise Ratio.

1 Also known as Occam’s razor, law of
parsimony, law of economy, and principle
of simplicity. The term “Ockham’s razor”
references William of Ockham, a 14th century
Franciscan friar and logician who purportedly
made abundant use of the principle. The
principle does not actually appear in any of
his extant writings and, in truth, little is known
about either the origin of the principle or its
originator. See, for example, “The Myth of
Occam’s Razor” by W. M. Thorburn, Mind,
1918, vol. 27, p. 345–353.
2 “Make all visual distinctions as subtle as
possible, but still clear and effective. ” Visual
Explanations by Edward R. Tufte, Graphics
Press, 1998, p. 73.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

• Advanced Search
• Preferences
• Language Tools
Advertise with Us - Search Solutions - News and Resources - Services & Tools
Jobs, Press, Cool Stuff
The Yamaha Compact Silent Electric
Cello is a minimalist cello with only
those portions touched by the player
represented. Musicians can hear
concert-quality cello sound through
headphones while creating little
external sound, or through an
amplifier and speakers for public
performances. The cello can also
be collapsed for easy transport
and storage.
While other Internet search services
were racing to add advertising and
ad hoc functions to their Web sites,
Google kept its design simple and
efficient. The result is the best
performing and easiest to use search
service on the Web.
The Taburet M Stacking Stool is
strong, comfortable, and stackable.
It is constructed from a single
piece of molded wood and has
no extraneous elements.
Ockham’s Razor 173
Web 	Images 	Groups 	Directory
Google Search 	I’m Feeling Lucky
Searching 2,469,940,685 web pages

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Ockham’s Razor** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Ockham’s Razor để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Form Follows Function, Horror Vacui, Mapping, and Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
