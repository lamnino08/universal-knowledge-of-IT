---
name: "Common Fate"
vi: "Nguyên lý chung hướng chuyển động"
summary: "Common Fate (Nguyên lý chung hướng chuyển động): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Common Fate (Nguyên lý chung hướng chuyển động)

> **Tóm tắt cốt lõi (Summary)**: Common Fate là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Elements that move in the same direction are perceived
to be more related than elements that move in different
directions or are stationary.
The principle of common fate is one of a number of principles referred to as
Gestalt principles of perception. It asserts that elements that move together in a
common direction are perceived as a single group or chunk, and are interpreted
as being more related than elements that move at different times or in different
directions. For example, a row of randomly arranged Xs and Os that is stationary
is naturally grouped by similarity, Xs with Xs, and Os with Os. However, if certain
elements in the row move in one direction, and other elements move in the
opposite direction, elements are grouped by their common motion and direction.1
Perceived relatedness is strongest when the motion of elements occurs at the
same time and velocity, and in the same direction. As any of these factors vary,
the elements are decreasingly related. One exception is when the motion exhibits
an obvious pattern or rhythm (e.g., wave patterns), in which case the elements
are seen as related. Although common fate relationships usually refer to moving
elements, they are also observed with static objects that flicker (i.e., elements that
alternate between brighter and darker states). For flickering elements, perceived
relatedness is strongest when the elements flicker at the same time, frequency,
and intensity, or when a recognizable pattern or rhythm is formed.2
Common fate relationships influence whether elements are perceived as figure or
ground elements. When certain elements are in motion and others are stationary,
the moving objects will be perceived as figure elements, and stationary ones
will be perceived as ground elements. When elements within a region move
together with the bounding edge of the region, the elements and the region will
be perceived as the figure. When elements within a region move together, but
the bounding edge of the region remains stationary or moves opposite to the
elements, the elements within the region will be perceived as the ground.3
Consider common fate as a grouping strategy when displaying information with
moving or flickering elements. Related elements should move at the same time,
velocity, and direction, or flicker at the same time, frequency, and intensity.
It is possible to group elements when these variables are dissimilar, but only
if the motion or flicker forms a recognizable pattern. When moving elements
within bounded regions, move the edges of the region in the same direction as
the elements to achieve a figure relationship or in the opposite direction as the
elements to achieve a ground relationship.
See also Figure-Ground Relationship and Similarity.

1 The seminal work on common fate is
“Untersuchungen zür Lehre von der Gestalt,
II” [Laws of Organization in Perceptual
Forms] by Max Wertheimer, Psychologische
Forschung, 1923, vol. 4, p. 301–350, reprinted
in A Source Book of Gestalt Psychology by
Willis D. Ellis (ed.), Routledge & Kegan Paul,
1999, p. 71v88.
2 See, for example, “Generalized Common Fate:
Grouping by Common Luminance Changes”
by Allison B. Sekuler and Patrick J. Bennett,
Psychological Science, 2001, Vol. 12(6), p.
437–444.
3 “Common Fate as a Determinant of Figure-
Ground Organization” by Joseph Lloyd Brooks,
Stanford-Berkeley Talk, 2000, Stanford
University, May 16, 2000.
Common Fate

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

DAL76
260 280
013 459
AAL427
200 263
004 440
USA990
200 225
038 440
VAL755
3300
031 459
DAL80
250C
014 440
FDX31
310 330
016 450
AAL215
290C
002 480
VAL1504
330C
028 465
NWA57
260C
020 440
NWA15
280C
018 440
AAL34
310C
003 430
VAL1
310C
027 480
USA442
200 231
037 440
Radar tracking displays use common
fate to group tracked aircraft with
key information about their identities
and headings.
The Xs and Os group by similarity
when stationary, such as Xs with Xs,
Os with Os. However, when a mix of
the Xs and Os move up and down in
a common fashion, they are grouped
primarily by common fate.
Common Fate 51
This object is being
tracked by radar.
The object and its
label are visually
grouped because they
are moving at the
same speed and in
the same direction.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Common Fate** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Common Fate để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Figure-Ground Relationship and Similarity
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
