---
name: "Defensible Space"
vi: "Không gian phòng vệ (Defensible Space)"
summary: "Defensible Space (Không gian phòng vệ (Defensible Space)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Defensible Space (Không gian phòng vệ (Defensible Space))

> **Tóm tắt cốt lõi (Summary)**: Defensible Space là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A space that has territorial markers, opportunities for
surveillance, and clear indications of activity and ownership.
Defensible spaces are used to deter crime. A defensible space is an area such as
a neighborhood, house, park, or office that has features that convey ownership
and afford easy and frequent surveillance. These features allow residents to
establish control over their private and community property, and ultimately deter
criminal activity. There are three key features of defensible spaces: territoriality,
surveillance, and symbolic barriers.1
Territoriality is the establishment of clearly defined spaces of ownership. Common
territorial features include community markers and gates to cultivate a community
identity and mark the collective territory of residents; visible boundaries such
as walls, hedges, and fences to create private yards; and privatization of public
services so that residents must take greater personal responsibility and ownership
(e.g., private trash cans instead of public dumpsters). These territorial elements
explicitly assign custodial responsibility of a space to residents, and communicate
to outsiders that the space is owned and protected.
Surveillance is the monitoring of the environment during normal daily activities.
Common surveillance features include external lighting; windows and doors that
open directly to the outside of first-floor dwellings; mailboxes located in open and
well-trafficked areas; and well-maintained courtyards, playgrounds, and walkways
that increase pedestrian activity and casual surveillance. These features make it
more difficult for people to engage in unnoticed activities.
Symbolic barriers are objects placed in the environment to create the perception
that a person’s space is cared for and worthy of defense. Common symbolic
barriers include picnic tables, swings, flowers, and lawn furniture—any symbol
that conveys that the owner of the property is actively involved in using and
maintaining the property. Note that when items that are atypical for a community
are displayed, it can sometimes symbolize affluence and act as a lure rather than
a barrier. Therefore, the appropriateness of various kinds of symbolic barriers must
be considered within the context of a particular community.2
Incorporate defensible space features in the design of residences, offices,
industrial facilities, and communities to deter crime. Clearly mark territories to
indicate ownership and responsibility; increase opportunities for surveillance and
reduce environmental elements that allow concealment; reduce unassigned open
spaces and services; and use typical symbolic barriers to indicate activity and use.
See also Control, Prospect-Refuge, Visibility, and Wayfinding.
1 The seminal works on defensible space are
Defensible Space: People and Design in the
Violent City, Macmillan, 1972; and Creating
Defensible Space, U.S. Department of
Housing and Urban Development, 1996, both
by Oscar Newman.
2 “Territorial Cues and Defensible Space
Theory: The Burglar’s Point of View” by Julie
E. MacDonald and Robert Gifford, Journal of
Environmental Psychology, 1989, vol. 9, p.
193–205.
Defensible Space

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Elements that indicate ownership
and improve surveillance enhance
the defensibility of a space. In this
case, the addition of community
markers and gating indicates a territory
that is owned by the community;
improved lighting and public benches
increase opportunities for casual
surveillance; and local fences,
doormats, shrubbery, and other
symbolic barriers clearly convey that
the space is owned and maintained.
Defensible Space 71
Before
After
Territoriality
Surveillance
Symbolic Barriers

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Defensible Space** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Defensible Space để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Control, Prospect-Refuge, Visibility, and Wayfinding
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
