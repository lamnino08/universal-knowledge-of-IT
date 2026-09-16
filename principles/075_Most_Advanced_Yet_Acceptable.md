---
name: "Most Advanced Yet Acceptable"
vi: "Tiên tiến nhất nhưng vẫn được chấp nhận (MAYA)"
summary: "Most Advanced Yet Acceptable (Tiên tiến nhất nhưng vẫn được chấp nhận (MAYA)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Most Advanced Yet Acceptable (Tiên tiến nhất nhưng vẫn được chấp nhận (MAYA))

> **Tóm tắt cốt lõi (Summary)**: Most Advanced Yet Acceptable là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A method for determining the most commercially viable
aesthetic for a design.1
What does it mean to create a successful design? Some define success in terms
of aesthetics, others in terms of function, and still others in terms of usability.
The noted industrial designer, Raymond Loewy, defined success in terms of
commercial performance — that is, sales. By this standard, Loewy believed that
aesthetic appeal was essentially a balancing act between two variables: familiarity
and uniqueness — or, in modern psychological parlance, typicality and
novelty — and to find the optimal balance between these variables was to find
the commercial sweet spot for success. According to Loewy, the sweet spot
could be identified using the Most Advanced Yet Acceptable (MAYA) principle,
which asserts that the most advanced form of an object or environment that is
still recognizable as something familiar will have the best prospects for com-
mercial success. Though Loewy generally equated “most advanced” with “most
streamlined,” a more accurate modern interpretation would be “most novel.”2
Although MAYA clearly has pragmatic appeal, the question as to its correctness
is an empirical one, and a growing body of research supports the principle.
People do indeed like the familiar, an observation supported by the exposure
effect, which claims that the appeal of objects and environments increases with
repeated exposures. People also like the novel, especially within design and
fine art circles — two communities that tend to value originality above all else.
Additionally, people tend to notice and remember novelty greater than typicality,
a phenomenon known as the von Restorff effect. Research assessing the relative
value of typicality and novelty suggests that the two variables seem to weigh
about equally in influencing perceptions of aesthetic appeal. The last question
is whether MAYA’s proposed point along the familiarity-novelty continuum is the
ideal one, and there is good evidence that Loewy got it pretty much right. When
dealing with everyone but design and art experts, the most novel design that is
still recognizable as a familiar object or environment is perceived to have the
greatest aesthetic appeal.3
Consider MAYA when designing for mass audiences. When introducing innovative
products that define a new category, consider incorporating elements that
reference familiar forms. In contexts where aesthetic assessments are made by
design or art experts (e.g., design competitions refereed by expert judges), MAYA
does not apply —in these cases, emphasize novelty, as it will be weighed more
heavily than typicality.4
See also Exposure Effect, Normal Distribution, and von Restorff Effect.
1 Also known as MAYA.
2 The seminal work on MAYA is Never Leave
Well Enough Alone by Raymond Loewy, The
John Hopkins University Press, 1951.
3 “‘Most Advanced, Yet Acceptable’: Typicality
and Novelty as Joint Predictors of Aesthetic
Preference in Industrial Design” by Paul
Hekkert, Dirk Snelders, and Piet C.W. van
Wieringen, British Journal of Psychology,
2003, vol. 94, p. 111–124. See also “Exposure
and Affect: Overview and Meta-Analysis of
Research, 1968–1987” by Robert Bornstein,
Psychological Bulletin, 1989, vol. 106, p.
265–289.
4 Though familiarity and typicality are similar and
generally correlate, they are distinct. Familiarity
refers to the level of past exposure (e.g., a
person sees a juicer every day). Typicality
refers to how recognizable a thing is for its type
(e.g., a new juicer is recognizable as a juicer
based on the appearance of past juicers).
Most Advanced Yet Acceptable

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Most Advanced Yet Acceptable 163
The traditional four-legged upholstered
chair served as the basic cognitive
prototype for office chairs for more
than fifty years.
The Aeron chair, introduced in 1992,
stretched this cognitive prototype for
most consumers. Its novel form and
high price were not acceptable to
most at that time. It would take several
years for norms to adjust and allow the
Aeron to become widely accepted.
The Variable Balans was introduced
in 1976. Its highly unique form and
approach to active sitting continues to
be too different for most consumers,
garnering positive attention almost
exclusively from the design community
where novelty is more highly valued.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Most Advanced Yet Acceptable** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Most Advanced Yet Acceptable để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Exposure Effect, Normal Distribution, and von Restorff Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
