---
name: "Horror Vacui"
vi: "Hội chứng sợ khoảng trắng (Horror Vacui)"
summary: "Horror Vacui (Hội chứng sợ khoảng trắng (Horror Vacui)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Horror Vacui (Hội chứng sợ khoảng trắng (Horror Vacui))

> **Tóm tắt cốt lõi (Summary)**: Horror Vacui là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Horror Vacui
A tendency to favor filling blank spaces with objects and
elements over leaving spaces blank or empty.
Horror vacui—a Latin expression meaning “fear of emptiness”—regards the
desire to fill empty spaces with information or objects. In style, it is the opposite
of minimalism. Though the term has varied meanings across different disciplines
dating back to Aristotle, today it is principally used to describe a style of art and
design that leaves no empty space. Examples include the paintings of artists Jean
Dubuffet and Adolf Wölfli, works of graphic designers David Carson and Vaughan
Oliver, and the cartoons of S. Clay Wilson and Robert Crumb. The style is also
commonly employed in various commercial media such as newspapers, comic
books, and websites.1
Recent research into how horror vacui is perceived suggests a general inverse
relationship between horror vacui and value perception—that is, as horror vacui
increases, perceived value decreases. For example, in a survey of more than 100
clothing stores that display merchandise in shop windows, the degree to which
the shop windows were filled with mannequins, clothes, price tags, and signage
was inversely related to the average price of the clothing and brand prestige of
the store. Bulk sales shops and chain stores tended to fill window displays to
the maximum degree possible, using every inch of real estate to display multiple
mannequins, stacks of clothes, and advertising promotions, whereas high-end
boutiques often used a single mannequin, no hanging or stacked clothes, no
signage, and no price tags—if passersby need to know the price, they presumably
could not afford it. This result is certainly consistent with common experience, but
somewhat surprising as lavish decoration is historically considered an indication of
affluence and luxury.
It may be that the inverse relationship is actually between the affluence of a
society and the perceived value associated with horror vacui—that is, for those
accustomed to having more, less is more, and for those accustomed to having
less, more is more. Others have speculated that the relationship is more a
function of education than affluence. This area of research is immature and much
follow-up is required to tease out the causal factors, but the preliminary findings
are compelling.2
Consider horror vacui in the design of commercial displays and advertising.
To promote associations of high value, favor minimalism for affluent and well-
educated audiences and horror vacui for poorer and less-educated audiences,
and vice versa. For information-rich media such as newspapers and websites,
employ information-organizing principles such as alignment and chunking to
retain the benefits of information-dense pages while mitigating horror vacui.
See also Alignment, Chunking, Ockham’s Razor, Progressive Disclosure, and
Signal-to-Noise Ratio.
1 Horror vacui is most notably associated with
the Italian-born critic Mario Praz, who used the
term to describe the cluttered interior design of
the Victorian age.
2 “Visualizing Emptiness” by Dimitri Mortelmans,
Visual Anthropology, 2005, vol. 18, p. 19–45.
See also The Sense of Order: A Study in
the Psychology of Decorative Art by Ernst
Gombrich, Phaidon, 1970.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Horror Vacui 129
Three shop windows with varying
levels of merchandise on display. The
perceived value of the merchandise
and prestige of the store are generally
inversely related to the visual
complexity of the display.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Horror Vacui** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Horror Vacui để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Alignment, Chunking, Ockham’s Razor, Progressive Disclosure, and
Signal-to-Noise Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
