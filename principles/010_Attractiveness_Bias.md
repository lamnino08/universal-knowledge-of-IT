---
name: "Attractiveness Bias"
vi: "Thiên kiến vẻ đẹp hấp dẫn"
summary: "Attractiveness Bias (Thiên kiến vẻ đẹp hấp dẫn): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Attractiveness Bias (Thiên kiến vẻ đẹp hấp dẫn)

> **Tóm tắt cốt lõi (Summary)**: Attractiveness Bias là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Attractiveness Bias
A tendency to see attractive people as more intelligent,
competent, moral, and sociable than unattractive people.1
Attractive people are generally perceived more positively than unattractive people.
They receive more attention from the opposite sex, receive more affection from
their mothers, receive more leniency from judges and juries, and receive more
votes from the electorate than do unattractive people. All other variables being
equal, attractive people are preferred in hiring decisions, and will make more
money doing the same work than unattractive people. The attractiveness bias is
a function of both biological and environmental factors.2
Biologically speaking, people are attractive when they exude health and fertility.
Good biological measures for health and fertility are average and symmetrical
facial features, and a waist-to-hip ratio in the ideal range (0.70 for women, 0.90 for
men). An absence of these features is thought to be an indicator of malnutrition,
disease, or bad genes; none of which are preferable attributes for a potential mate.
Biological factors of attraction are innate and true across cultures. For example,
in studies presenting images of attractive and unattractive people to babies (two-
months-old and six-months-old), the babies looked longer at the attractive people
regardless of their gender, age, or race.3
Environmentally speaking, men are attracted to women when they exaggerate
socially acknowledged features of sexuality (e.g., lipstick to exaggerate lips); and
women are attracted to men when they appear to possess wealth and power (e.g.,
expensive automobiles). For example, in studies presenting images of attractive
and unattractive people to men and women, along with descriptions of their
occupations, women preferred unattractive men with high-paying occupations
equally to attractive men with medium-paying occupations. However, men never
preferred unattractive women regardless of their financial status. Environmental
factors of attraction vary considerably across cultures.4
Consider the attractiveness bias in design contexts involving images of people,
such as marketing and advertising. When the presentation of attractive women is
a key element of a design, use renderings or images of women with waist-to-hip
ratios of approximately 0.70, accented by culturally appropriate augmentations
of sexual features. When the presentation of attractive men is a key element of a
design, use renderings or images of men with waist-to-hip ratios of approximately
0.90, and visible indicators of wealth or status (e.g., expensive clothing).
See also Anthropomorphic Form, Baby-Face Bias, Most Average Facial
Appearance Effect, Red Effect, and Waist-to-Hip Ratio.

1 Also known as look-ism.
2 The seminal work on the attractiveness bias
is “What Is Beautiful Is Good” by Karen Dion,
Ellen Berscheid, and Elaine Walster, Journal
of Personality and Social Psychology, 1972,
vol. 24(3), p. 285–290. A nice contemporary
review of the attractiveness bias research is
“Maxims or Myths of Beauty? A Meta-analytic
and Theoretical Review” by Judith H. Langlois,
et al., Psychological Bulletin, 2000, vol. 126(3),
p. 390–423.
3 See, for example, “Baby Beautiful: Adult
Attributions of Infant Competence as a
Function of Infant Attractiveness” by Cookie
W. Stephan and Judith H. Langlois, Child
Development, 1984, vol. 55, p. 576–585.
4 Survival of the Prettiest: The Science of Beauty
by Nancy Etcoff, Anchor Books, 2000.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

The first presidential debate between
Richard Nixon and John Kennedy
(1960) is a classic demonstration of
the attractiveness bias. Nixon was
ill and running a fever. He wore
light colors and no makeup, further
whitening his already pale complexion
and contrasting his five-o’clock
shadow. Kennedy wore dark colors,
makeup, and practiced his delivery in
a studio prior to the debate. People
who listened to the debate by radio
believed Nixon to be the winner.
However, people who watched the
debate on TV came to a very different
conclusion.
Attractiveness Bias 33

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Attractiveness Bias** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Attractiveness Bias để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Anthropomorphic Form, Baby-Face Bias, Most Average Facial
Appearance Effect, Red Effect, and Waist-to-Hip Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
