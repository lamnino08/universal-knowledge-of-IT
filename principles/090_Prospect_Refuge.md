---
name: "Prospect-Refuge"
vi: "Triển vọng - Trú ẩn (Prospect-Refuge)"
summary: "Prospect-Refuge (Triển vọng - Trú ẩn (Prospect-Refuge)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Prospect-Refuge (Triển vọng - Trú ẩn (Prospect-Refuge))

> **Tóm tắt cốt lõi (Summary)**: Prospect-Refuge là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Prospect-Refuge
A tendency to prefer environments with unobstructed views
(prospects) and areas of concealment and retreat (refuges).
People prefer environments where they can easily survey their surroundings and
quickly hide or retreat to safety if necessary. Environments with both prospect
and refuge elements are perceived as safe places to explore and dwell, and
consequently are considered more aesthetic than environments without these
elements. The principle is based on the evolutionary history of humans, reasoning
that environments with ample prospects and refuges increased the probability of
survival for pre-humans and early humans.1
The prospect-refuge principle suggests that people prefer the edges, rather than
middles of spaces; spaces with ceilings or covers overhead; spaces with few
access points (protected at the back or side); spaces that provide unobstructed
views from multiple vantage points; and spaces that provide a sense of safety and
concealment. The preference for these elements is heightened if the environment
is perceived to be hazardous or potentially hazardous.
Environments that achieve a balance between prospects and refuges are the
most preferred. In natural environments, prospects include hills, mountains, and
trees near open settings. Refuges include enclosed spaces such as caves, dense
vegetation, and climbable trees with dense canopies nearby. In human-created
environments, prospects include deep terraces and balconies, and generous use
of windows and glass doors. Refuges include alcoves with lowered ceilings and
external barriers, such as gates and fences.2
The design goal of prospect-refuge can be summarized as the development of
spaces where people can see without being seen. Consider prospect-refuge in
the creation of landscapes, residences, offices, and communities. Create multiple
vantage points within a space, so that the internal and external areas can be easily
surveyed. Make large, open areas more appealing by using screening elements
to create partial refuges with side- and back-barriers while maintaining clear lines
of sight (e.g., shrubbery, partitions). Balance the use of prospect and refuge
elements for optimal effect—e.g., sunken floors and ceilings that open to larger
spaces enclosed by windows and glass doors.
See also Biophilia Effect, Cathedral Effect, Defensible Space, Savanna Preference,
and Wayfinding.

1 The seminal work on prospect-refuge theory is
The Experience of Landscape by Jay Appleton,
John Wiley & Sons, 1975.
2 See, for example, The Wright Space: Pattern
and Meaning in Frank Lloyd Wright’s Houses
by Grant Hildebrand, University of Washington
Press, 1991.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

This section of an imaginary café
highlights many of the practical
applications of the prospect-refuge
principle. The entry is separated from
the interior by a greeting station,
and the ceiling is lowered to create a
temporary refuge for waiting patrons.
As the interior is accessed, the
ceiling raises and the room opens
up with multiple, clear lines of sight.
A bar area is set against the far
wall with a raised floor and lowered
ceilings, creating a protected perch
to view interior and exterior areas.
High-backed booths and partial
screens provide refuge with minimal
impediment to prospect. Windows are
tinted or mirrored, allowing patrons
to survey the exterior without being
seen. Shrubbery surrounds the
exterior as a practical and symbolic
barrier, preventing outsiders from
getting too close.
Prospect-Refuge 193
Low ceiling
Low ceiling
High ceiling
Divider between
dining areas
Raised floor Divider between
entry and main area
High-backed booths
Shrubbery
Tinted windows

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Prospect-Refuge** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Prospect-Refuge để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Biophilia Effect, Cathedral Effect, Defensible Space, Savanna Preference,
and Wayfinding
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
