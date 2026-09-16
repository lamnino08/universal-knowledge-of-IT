---
name: "Comparison"
vi: "Nguyên lý so sánh đối chiếu"
summary: "Comparison (Nguyên lý so sánh đối chiếu): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
  - decision
---

# Universal Design Principle: Comparison (Nguyên lý so sánh đối chiếu)

> **Tóm tắt cốt lõi (Summary)**: Comparison là một nguyên lý thiết kế then chốt thuộc nhóm **learning, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A method of illustrating relationships and patterns in
system behaviors by representing two or more system
variables in a controlled way.
People understand the way the world works by identifying relationships and
patterns in or between systems. One of the most powerful methods of identifying
and understanding these relationships is to represent information in controlled
ways so that comparisons can be made. Key techniques for making valid
comparisons are apples to apples, single contexts, and benchmarks.1
Apples to Apples
Comparison data should be presented using common measures and common
units. For example, when comparing crime rates of different countries, it is
necessary to account for differences in variables such as population, types of laws,
and level of law enforcement. Otherwise, conclusions based on the comparison
will be unreliable. Common methods of ensuring apples-to-apples comparisons
include clearly disclosing details of how variables were measured, making
corrections to the data as necessary to eliminate confounding variables, and
representing the variables using the same graphical and numerical standards.
Single Context
Comparison data should be presented in a single context, so that subtle differences
and patterns in the data are detectable. For example, the ability to detect patterns
across multiple graphs is lower if the graphs are located on separate pages versus
the same page. Common methods of representing information in single contexts
include the use of a small number of displays that combine many variables (versus
many separate displays), and multiple small views of system states (known as small
multiples) in a single display (versus multiple displays).
Benchmarks
Claims about evidence or phenomena should be accompanied by benchmark
variables so that clear and substantive comparisons can be made. For example,
claims about the seriousness of the size of the U.S. debt are meaningful only
when accompanied by benchmark information about U.S. gross national product
(GNP); a debt can appear serious when depicted as a quantity, but irrelevant when
presented as a percentage of GNP. Common types of benchmark data include past
performance data, competitor data, or data from well-accepted industry standards.
Use comparisons to convincingly illustrate patterns and relationships. Ensure
that compared variables are apples to apples by measuring and representing
variables in common ways, correcting for confounds in the data as necessary. Use
multivariate displays and small multiples to present comparisons in single contexts
when possible. Use benchmarks to anchor comparisons and provide a point of
reference from which to evaluate the data.
See also Garbage In–Garbage Out, Layering, and Signal-to-Noise Ratio.

1 See, for example, Visual Explanations,
Graphics Press, 1998; and Envisioning
Information, Graphics Press, 1990 both by
Edward R. Tufte.
Comparison

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

This is a modified version of Florence
Nightingale’s famous Coxcomb
graphs. The graphs are composed
of twelve wedges, each representing
a month. Additionally, each wedge
has three layers representing three
different causes of death. A quick
review of the graphs reveals that the
real threat to British troops was not the
Russians, but cholera, dysentery, and
typhus. The graphs also convincingly
illustrate the impact of improved
hygienic practices at military camps
and hospitals, which were aggressively
implemented beginning in March
1855. The graphs make apples-to-
apples comparisons, representing the
same variable (death rates) the same
way (area of the wedge).
The graphs are multivariate, integrating
a number of key variables so that
patterns and relationships in the data
can be studied within one context.
Deaths resulting from war wounds
serve as a compelling benchmark to
illustrate the significance of disease,
as does the earlier graph for the
later graph. The graphs have been
corrected based on original data
published in Nightingale’s Notes on
Matters Affecting the Health, Efficiency
and Hospital Administration of the
British Army, 1858.
Comparison 53
Diagram of the Causes of Mortality
in the Army in the East
April 1854 to March 1855 	April 1855 to March 1856
Death from wounds in battle
Death from other causes
Death from disease
May
Apr 1854
June
	July
Aug
Sept
Oct
Nov
Dec
Jan 1855
Feb
Mar 1855
Crimea
Bulgaria
May
Apr 1855
June
July
Aug
Sept
Oct
Nov
	Dec
Jan 1856
Feb
Mar 1856

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Comparison** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Comparison để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Garbage In–Garbage Out, Layering, and Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
