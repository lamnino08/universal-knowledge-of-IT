---
name: "Design by Committee"
vi: "Thiết kế theo hội đồng"
summary: "Design by Committee (Thiết kế theo hội đồng): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Design by Committee (Thiết kế theo hội đồng)

> **Tóm tắt cốt lõi (Summary)**: Design by Committee là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Design by Committee
A design process based on consensus building,
group decision making, and extensive iteration.
It is a commonly held view that good design results when projects are driven
by an autocratic leader, and bad design results when projects are driven by
democratized groups.1 Many find this notion of an alpha leader romantically
appealing, believing that great design requires a tyrannical “Steve Jobs” at the
helm to be successful. This notion is, at best, an oversimplification, and in many
cases it is simply incorrect.
Design by dictator is preferred when projects are time-driven, requirements are
relatively straightforward, consequences of error are tolerable, and stakeholder
buy-in is unimportant. It should be noted that with the exception of inventors,
celebrity designers, and entrepreneurial start-ups, virtually all modern design
is at some level design by committee (e.g., clients, brand managers, etc.). The
belief that great design typically comes from dictators is more myth than reality.
Design by committee is preferred when projects are quality-driven, requirements
are complex, consequences of error are serious, or stakeholder buy-in is impor-
tant. For example, NASA employs a highly bureaucratized design process for each
mission, involving numerous working groups, review committees, and layers of
review from teams of various specializations. The process is slow and expensive,
but the complexity of the requirements is high, the consequences of error are
severe, and the need for stakeholder buy-in is critical. Virtually every aspect of
mission technology is a product of design by committee.
Design by committee is optimal when committee members are diverse, bias
and influence among committee members is minimized, local decision-making
authority is encouraged operating within an agreed upon global framework,
member input and contributions are efficiently collected and shared, ideal group
sizes are employed (working groups contain three members, whereas review
boards and decision-making panels contain seven to twelve members), and a
simple governance model is adopted to facilitate decision making and ensure that
the design process cannot be delayed or deadlocked.2
Consider design by committee when quality, error mitigation, and stakeholder
acceptance are primary factors. Consider design by dictator when an aggressive
timeline is the primary factor. Favor some form of design by committee for
most projects, as it generally outperforms design by dictator on most critical
measures with lower overall risk of failure — bad dictators are at least as common
as good dictators, and design by dictator tends to lack the error correction and
organizational safety nets of committee-based approaches. Autocracy is linear and
fast, but risky and prone to error. Democracy is iterative and slow, but careful and
resistant to error. Both models have their place depending on the circumstances.3
See also Development Cycle, Iteration, and Most Advanced Yet Acceptable.
1 See, for example, “Designed for Life” by
Wendy Grossman, New Scientist, October 5,
2002, vol. 176, p. 2363.
2 For information regarding the optimal factors
supporting group decision making and
problem solving, see “Groups Perform Better
Than the Best Individuals on Letters-to-
Numbers Problems: Informative Equations
and Effective Strategies” by Patrick Laughlin,
Megan Zander, Erica Knievel, et al., Journal of
Personality and Social Psychology, 2003, vol.
85(4), p. 684–694. See also “To Err Is Human,
to Correct for It Divine: A Meta-Analysis of
Research Testing the Functional Theory of
Group Decision-Making Effectiveness” by Marc
Orlitzky and Randy Hirokawa, Small Group
Research, June 2001, vol. 32(3), p. 313–341.
3 For a popular treatment of the power of group-
and committee-based decision making, see
The Wisdom of Crowds by James Surowiecki,
Anchor, 2005.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Design by Committee 75
The striking original design for
Freedom Tower (left) came
from Daniel Libeskind using a
design process that can be aptly
characterized as design by dictator.
However, the requirements of the
building that would take the place
of the World Trade Center towers
were extraordinarily complex, the
consequences of getting the design
wrong unacceptable, and the number
of passionate stakeholders great.
Given these conditions, Freedom
Tower was destined to be designed
by committee. As the design iterated
through the various commercial,
engineering, security, and political
factions, idiosyncrasies were averaged
out — a standard byproduct of design
by committee. The final design (right)
is less visually interesting, but it is, by
definition, a superior design.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Design by Committee** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Design by Committee để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Development Cycle, Iteration, and Most Advanced Yet Acceptable
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
