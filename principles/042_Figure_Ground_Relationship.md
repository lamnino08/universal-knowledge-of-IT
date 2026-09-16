---
name: "Figure-Ground Relationship"
vi: "Quan hệ hình - nền (Figure-Ground)"
summary: "Figure-Ground Relationship (Quan hệ hình - nền (Figure-Ground)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Figure-Ground Relationship (Quan hệ hình - nền (Figure-Ground))

> **Tóm tắt cốt lõi (Summary)**: Figure-Ground Relationship là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Elements are perceived as either figures (objects of focus)
or ground (the rest of the perceptual field).
The figure-ground relationship is one of several principles referred to as Gestalt
principles of perception. It asserts that the human perceptual system separates
stimuli into either figure elements or ground elements. Figure elements are the
objects of focus, and ground elements compose an undifferentiated background.
This relationship can be demonstrated with both visual stimuli, such as photographs,
and auditory stimuli, such as soundtracks with dialog and background music.1
When the figure and ground of a composition are clear, the relationship is stable;
the figure element receives more attention and is better remembered than the
ground. In unstable figure-ground relationships, the relationship is ambiguous
and can be interpreted in different ways; the interpretation of elements alternates
between figure and ground.
The visual cues that determine which elements will be perceived as figure and
which as ground are:
• The figure has a definite shape, whereas the ground is shapeless.
• The ground continues behind the figure.
• The figure seems closer with a clear location in space, whereas the ground
seems farther away and has no clear location in space.
• Elements below a horizon line are more likely to be perceived as figures,
whereas elements above a horizon line are more likely to be perceived
as ground.
• Elements in the lower regions of a design are more likely to be perceived
as figures, whereas elements in the upper regions are more likely to be
perceived as ground.2
Clearly differentiate between figure and ground in order to focus attention and
minimize perceptual confusion. Ensure that designs have stable figure-ground
relationships by incorporating the appropriate visual cues listed above. Increase the
probability of recall of key elements by making them figures in the composition.
See also Gutenberg Principle, Law of Prägnanz, Top-Down Lighting Bias, and
Visuospacial Resonance.
1 The seminal work on the figure-ground
relationship is “Synoplevede Figurer” [Figure
and Ground] by Edgar Rubin, Gyldendalske,
1915, translated and reprinted in Readings
in Percep-tion by David C. Beardslee and
Michael Werth-eimer, D. Van Nostrand, 1958,
p. 194–203.
2 “Lower Region: A New Cue for Figure-Ground
Assignment” by Shaun P. Vecera, Edward K.
Vogel, and Geoffrey F. Woodman, Journal of
Experimental Psychology: General, 2002, vol.
131(2), p. 194–205.
Figure-Ground Relationship

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Figure-Ground Relationship 97
The Rubin vase is unstable because
it can be perceived as a white vase
on a black background or two black
faces looking at each other on a
white background.
Initially, there is no stable figure-
ground relationship in this image.
However, after a moment, the
Dalmatian pops out and the figure-
ground relationship stabilizes.
Placing the spa name below the
horizon line in the logo makes it a
figure element—it will receive more
attention and be better remembered
than the design that places the name
at the top of the logo.
Placing the logo at the bottom of the
page makes it a figure element—it
will receive more attention and will be
better remembered than the logo at
the top of the page.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Figure-Ground Relationship** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Figure-Ground Relationship để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Gutenberg Principle, Law of Prägnanz, Top-Down Lighting Bias, and
Visuospacial Resonance
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
