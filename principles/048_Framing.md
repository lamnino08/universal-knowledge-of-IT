---
name: "Framing"
vi: "Hiệu ứng đóng khung (Framing)"
summary: "Framing (Hiệu ứng đóng khung (Framing)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Framing (Hiệu ứng đóng khung (Framing))

> **Tóm tắt cốt lõi (Summary)**: Framing là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Framing
A technique that influences decision making and judgment
by manipulating the way information is presented.
Framing is the use of images, words, and context to manipulate how people think
about something. Information can be presented in such a way as to emphasize
the positive (e.g., glass is half-full) or the negative (e.g., glass is half-empty). The
type of frame used to present information dramatically affects how people make
decisions and judgments, and is consequently a powerful influencer of behavior.
News media, politicians, propagandists, and advertisers all commonly use framing
(knowingly or unknowingly) with great effect. 1
In October 2002, Russian Special Forces used a sedating gas to knock out
Chechen rebels who were holding over 750 hostages captive in the Moscow
Theater. The gas prevented the rebels from setting off explosives and killing all
of the hostages, but the gas itself caused the death of well over 100 hostages.
Newspapers throughout the world reported the incident in basically one of two
ways: Gas Kills Over 100 Hostages, or Gas Saves Over 500 Hostages. This event
is tragic no matter how it is presented, but judgment of the Russian efforts to free
the hostages is greatly influenced by the frame of its presentation. The negative
frame emphasizes the lives lost, and presents the information in a way that
suggests the Russians bungled the affair. The positive frame emphasizes the lives
saved, and presents the information in a way that suggests the Russians cleverly
salvaged a seemingly intractable situation. Similar positive and negative frames are
typically used in advertising. For example, it is common to see yogurt advertised
as 95 percent fat free, rather than 5 percent fat rich; and tobacco legislation has
been defeated more than once by framing the legislation as a matter of taxation,
instead of a matter of public health.
Positive frames tend to elicit positive feelings, and result in proactive and risk-
seeking behaviors. Negative frames tend to elicit negative feelings, resulting in
reactive and risk-avoiding behaviors. Stress and time pressures amplify these
behaviors, a phenomenon frequently exploited in high pressure sales: present a
product in a positive frame, present competitors in a negative frame, and time-
bound the decision to pressure the buy. However, when people are exposed to
multiple conflicting frames, the framing effect is neutralized, and people think and
act consistently with their own beliefs.
Use framing to elicit positive or negative feelings about a design, and to influence
behaviors and decision-making. Use positive frames to move people to action
(e.g., make a purchase) and negative frames to move people to inaction (e.g.,
prevent use of illegal drugs). To maintain a strong framing effect, make sure that
frames are not conflicting. Conversely, neutralize framing effects by presenting
multiple conflicting frames.
See also Expectation Effect, Exposure Effect, and Scarcity.
1 The seminal work on framing is “The Framing
of Decisions and the Psychology of Choice” by
Amos Tversky and Daniel Kahneman, Science,
1981, vol. 211, p. 453–458. A nice treatment
of the subject is The Psychology of Judgment
and Decision Making by Scott Plous, McGraw-
Hill, 1993.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The Ohio Dry Campaign of 1918 is
a case study in framing. Prohibition
advocates framed the issue as either
supporting prohibition of alcohol or
supporting waste, poverty, crime,
treason, and so on. The campaign
was successful in turning public
opinion, and resulted in passage of
prohibition legislation in 1918. Similar
framing tactics are common today.
For example, abortion-rights advocates
frame their position as prochoice
and their opponents’ as antichoice;
abortion-rights critics frame their
position as prolife and their opponents’
as anti-life or proabortion.
Framing 109

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Framing** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Framing để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Expectation Effect, Exposure Effect, and Scarcity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
