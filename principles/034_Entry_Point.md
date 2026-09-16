---
name: "Entry Point"
vi: "Điểm khởi đầu tiếp cận (Entry Point)"
summary: "Entry Point (Điểm khởi đầu tiếp cận (Entry Point)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - appeal
---

# Universal Design Principle: Entry Point (Điểm khởi đầu tiếp cận (Entry Point))

> **Tóm tắt cốt lõi (Summary)**: Entry Point là một nguyên lý thiết kế then chốt thuộc nhóm **usability, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

A point of physical or attentional entry into a design.
People do judge books by their covers, Internet sites by their first pages, and
buildings by their lobbies. This initial impression of a system or environment
greatly influences subsequent perceptions and attitudes, which then affects the
quality of subsequent interactions. This impression is largely formed at the entry
point to a system or environment. For example, entering many Internet sites
entails going through a slow-loading splash screen, followed by a slow-loading
main page, followed by several pop-up windows with advertisements—all this to
enter a site that may or may not have the information the person was looking for.
Such errors in entry point design annoy visitors who make it through, or deter
visitors altogether. Either way, it does not promote additional interaction. The key
elements of good entry point design are minimal barriers, points of prospect, and
progressive lures.1
Minimal Barriers
Barriers should not encumber entry points. Examples of barriers to entry are highly
trafficked parking lots, noisy displays with many unnecessary elements, sales-
people standing at the doors of retail stores, or anything that impedes people from
getting to and moving through an entry point. Barriers can be aesthetic as well as
functional in nature. For example, a poorly maintained building front or landscape
is an aesthetic barrier to entry.
Points of Prospect
Entry points should allow people to become oriented and clearly survey available
options. Points of prospect include store entrances that provide a clear view of
store layout and aisle signs, or Internet pages that provide good orientation cues
and navigation options. Points of prospect should provide sufficient time and
space for a person to review options with minimal distraction or disruption—i.e.,
people should not feel hurried or crowded by their surroundings or other people.
Progressive Lures
Lures should be used to attract and pull people through the entry point. Progressive
lures can be compelling headlines from the front page of a newspaper, greeters
at restaurants, or the display of popular products or destinations (e.g., restrooms)
just beyond the entry point of a store. Progressive lures get people to incrementally
approach, enter, and move through the entry point.
Maximize the effectiveness of the entry point in a design by reducing barriers,
establishing clear points of prospect, and using progressive lures. Provide
sufficient time and space for people to review opportunities for interaction at the
entry point. Consider progressive lures like highlighting, entry point greeters, and
popular offerings visibly located beyond the entry point to get people to enter and
progress through.
See also Immersion, Prospect-Refuge, and Wayfinding.
1 See, for example, Why We Buy: The Science
of Shopping by Paco Underhill, Touchstone
Books, 2000; Hotel Design, Planning, and
Development by Walter A. Rutes, Richard H.
Penner, Lawrence Adams, W. W. Norton &
Company, 2001; and “The Stanford-Poynter
Eyetracking Study” by Marion Lewenstein,
Greg Edwards, Deborah Tatar, and Andrew
DeVigal, http://www.poynterextra.org.
Entry Point

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Entry Point 81
Apple Computer retail stores maintain
the high standards of design excellence
for which Apple is known. The stores
appear more like museums than
retail shops, creating tempting visual
spectacles that are hard to pass by.
The redesign of the Wall Street Journal
creates a clear entry point to each
edition by highlighting the region of
the page containing news summaries.
The summaries also act as a point of
prospect, allowing readers to quickly
scan for stories of interest with no
competing visual barriers. Page
references on select summaries act
as progressive lures, leading readers
to the full articles in different sections
of the paper.
A glass front
eliminates visual barriers.
A large point of prospect is provided
after entry to support orientation
and decision making.
The use of glass
minimizes visual barriers.
A small set of glass stairs at the entry point
acts as a lure, creating the impression
of entering a special place.
A large glass staircase acts as a secondary
lure, creating the impression of entering
another special space.
Products line the periphery of the
space, offering clear options
from the point of prospect.
Apple Retail Store
Level 1

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Entry Point** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Entry Point để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Immersion, Prospect-Refuge, and Wayfinding
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
