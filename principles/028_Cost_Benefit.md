---
name: "Cost-Benefit"
vi: "Chi phí - Lợi ích (Cost-Benefit)"
summary: "Cost-Benefit (Chi phí - Lợi ích (Cost-Benefit)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
  - usability
---

# Universal Design Principle: Cost-Benefit (Chi phí - Lợi ích (Cost-Benefit))

> **Tóm tắt cốt lõi (Summary)**: Cost-Benefit là một nguyên lý thiết kế then chốt thuộc nhóm **decision, usability**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

An activity will be pursued only if its benefits are equal to
or greater than the costs.
From a design perspective, the cost-benefit principle is typically used to assess
the financial return associated with new features and elements. The cost-benefit
principle can also be applied to determine design quality from a user perspective.
If the costs associated with interacting with a design outweigh the benefits, the
design is poor. If the benefits outweigh the costs, the design is good. For example,
walking some distance to see a museum exhibit constitutes a cost. The level of
interest in the exhibit constitutes a benefit. Thus, if the level of interest outweighs
the cost of the walk, the exhibit design is good.
The quality of every design aspect can be measured using the cost-benefit
principle. How much reading is too much to get the point of a message? How
many steps are too many to set the time and date of a video recorder? How
long is too long for a person to wait for a Web page to download? The answer
to all of these questions is that it depends on the benefits of the interaction. For
example, the often-cited maximum acceptable download time for pages on the
Internet is ten seconds. However, the acceptability of download time is a function
of the benefits provided by the downloaded page. A high-benefit page can more
than compensate for the cost of a download taking longer than ten seconds.
Conversely, a low-benefit page cannot compensate the cost of any download time.
Reducing interaction costs does improve the quality of the design, but to simply
design within cost limits without consideration of the interaction benefits misses
the point of design altogether—i.e., to provide benefit.
A common mistake regarding application of the cost-benefit principle is to
presume which aspects of a system will be perceived as costs, and which will
be perceived as benefits. For example, new design features or elements that
excite designers are often never used or even noticed by people who interact with
the design. In many cases, such features and elements increase the design’s
interaction costs by adding complexity to the system. In order to avoid this,
observe people interacting with the design or similar designs in the actual target
environment. Focus groups and usability tests are valuable in assessing the cost-
benefits of a design during development, when natural observation is not possible.
Consider the cost-benefit principle in all aspects of design. Do not make design
decisions based on cost parameters alone without due consideration of the
benefits realized from interactions. Verify cost-benefit perceptions of target
populations through careful observations, focus groups, and usability tests.
See also 80/20 Rule, Aesthetic-Usability Effect, and Expectation Effect.
Cost-Benefit

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

From a user perspective, Internet
advertising via pop-up windows
is all cost and no benefit. If the
advertisements were properly
designed to minimize cost and
maximize benefit, people would
be more likely to pay attention and
form positive associations.
These banner advertisements
demonstrate one method of improving
the cost-benefit of Internet advertising:
creative interactivity. Whether shooting
viruses, playing slots, or engaging in
word play, these advertisements use
entertainment to compensate people
for their time and attention.
Cost-Benefit 69
Do you want your free gift that
has been valued at $50?
Cancel 	OK

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Cost-Benefit** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Cost-Benefit để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Aesthetic-Usability Effect, and Expectation Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
