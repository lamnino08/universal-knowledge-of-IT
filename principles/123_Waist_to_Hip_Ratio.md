---
name: "Waist-to-Hip Ratio"
vi: "Tỷ lệ eo trên hông"
summary: "Waist-to-Hip Ratio (Tỷ lệ eo trên hông): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Waist-to-Hip Ratio (Tỷ lệ eo trên hông)

> **Tóm tắt cốt lõi (Summary)**: Waist-to-Hip Ratio là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Waist-to-Hip Ratio
A preference for a particular ratio of waist size to hip size
in men and women.
The waist-to-hip ratio is a primary factor for determining attractiveness for
men and women. It is calculated by dividing the circumference of the waist
(narrowest portion of the midsection) by the circumference of the hips (area of
greatest protrusion around the buttocks). Men prefer women with a waist-to-hip
ratio between .67 and .80. Women prefer men with a waist-to-hip ratio between
0.85 and 0.95.1
The waist-to-hip ratio is primarily a function of testosterone and estrogen levels,
and their effect on fat distribution in the body. High estrogen levels result in low
waist-to-hip ratios, and high testosterone levels result in high waist-to-hip ratios.
Human mate selection preferences likely evolved to favor visible indicators of
these hormone levels (i.e., waist-to-hip ratios), as they are reasonably indicative of
health and reproductive potential.2
For men, attraction is primarily a function of physical appearance. Women who
are underweight or overweight are generally perceived as less attractive, but in all
cases women with waist-to-hip ratios approximating 0.70 are perceived as the most
attractive for their respective weight group. For women, attraction is a function of both
physical appearance and financial status. Financial status is biologically important
because it ensures a woman of security and status for herself and her children.
However, as women become increasingly independent with resources of their
own, the strength of financial status as a factor in attraction diminishes. Similarly,
women of modest resources may be attracted to men of low financial status when
their physical characteristics indicate strong male features like dominance and
masculinity (e.g., tall stature), but men with both high waist-to-hip ratios and high
financial status are perceived as the most desirable.
The waist-to-hip ratio has design implications for the depiction of the human
form. When the presentation of attractive women is a key element of a design, use
renderings or images of women with waist-to-hip ratios of approximately 0.70. When
the presentation of attractive men is a key element of a design, use renderings or
images of men with waist-to-hip ratios of approximately 0.90, strong male features,
and visible indicators of wealth or status (e.g., expensive clothing).
See also Anthromorphic Form, Attractiveness Bias, Baby-Face Bias, and
Golden Ratio.

1 The seminal work on the waist-to-hip ratio
is “Adaptive Significance of Female Physical
Attractiveness: Role of Waist-to-Hip Ratio,”
Journal of Personality and Social Psychology,
1993, vol. 65, p. 293–307; and “Female
Judgment of Male Attractiveness and
Desirability for Relationships: Role of Waist-
to-Hip Ratio and Financial Status,” Journal of
Personality and Social Psychology, 1995, vol.
69, p. 1089–1101, both by Devendra Singh.
2 While preferences for particular features like
body weight or breast size have changed over
time, the preferred waist-to-hip ratios have
remained stable. For example, in analyzing the
measurements of Playboy centerfolds since
the 1950s and Miss America winners since the
1920s, researchers discovered that the waist-
to-hip ratios remained between 0.68 and 0.72
despite a downward trend in body weight.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

When asked to select the most
attractive figures from renderings of
men and women of varying weights
and body types, people favored
male C and female A, corresponding
to waist-to-hip ratios of 0.90 and
0.70, respectively.
The world famous Adel Rootstein
mannequins have changed to match
the ideal look and body type of men
and women for over five decades
(1960s - 2000s). The waist-to-hip
ratios of the mannequins, however,
have not changed—they have
remained constant at around 0.90
for men, and 0.70 for women.
Waist-to-Hip Ratio 259

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Waist-to-Hip Ratio** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Waist-to-Hip Ratio để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Anthromorphic Form, Attractiveness Bias, Baby-Face Bias, and
Golden Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
