---
name: "Uncanny Valley"
vi: "Thung lũng kỳ dị (Uncanny Valley)"
summary: "Uncanny Valley (Thung lũng kỳ dị (Uncanny Valley)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Uncanny Valley (Thung lũng kỳ dị (Uncanny Valley))

> **Tóm tắt cốt lõi (Summary)**: Uncanny Valley là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Uncanny Valley
Anthropomorphic forms are appealing when they are
dissimilar or identical to humans, but unappealing when
they are very similar to humans.
Anthropomorphic forms are generally appealing to humans. However, when a
form is very close but not identical to a healthy human — as with a mannequin or
computer-generated renderings of people — the form tends to become distinctly
unappealing. This sharp decline in appeal is called the “uncanny valley,” a
reference to the large valley or dip in the now classic graph presented by Masahiro
Mori in 1970.1 Though some have disputed the existence of the effect altogether,
attributing any negative affective response to a simple lack of familiarity with artificial
and rendered likenesses, more recent empirical research suggests the uncanny
valley is a real phenomenon. The cause likely regards innate, subconscious
mechanisms evolved for pathogen avoidance — that is, detecting and avoiding
people who are sick or dead.2
Although a full understanding of the variables required to take an anthropomorphic
likeness into the uncanny valley has not yet been realized, some conditions have
been identified. The strength of the negative reaction seems to correspond to the
fidelity of the likeness — a highly realistic likeness that is identifiable as artificial
will evoke a stronger negative reaction than a less realistic likeness. Abnormally
proportioned or positioned facial features, asymmetry of facial features, subtleties
of eye movement, and unnatural skin complexions are all sufficient conditions to
trigger uncanny valley effects.
Although the uncanny valley is generally observed by animators and roboticists,
there are plenty of examples where the caveats of the principle are not abided.
For example, director Robert Zemeckis decided to depict computer-generated
characters with a high degree of realism for the movie The Polar Express. The
resulting effect was both impressively realistic and eerie. The movie raised
awareness of what is called “dead eye syndrome,” where the lack of eye
movements called saccades made the characters look zombielike, taking the Polar
Express straight through the uncanny valley. Another example is found in retail
contexts. There is a general perception among retailers that the effectiveness of
mannequins is a function of their realism. However, barring a mannequin that is
indistinguishable from a real person, the uncanny valley suggests that retailers
would be better served by more abstract versus highly realistic mannequins.
Consider the uncanny valley when representing and animating anthropomorphic
forms. Opt for more abstract versus realistic anthropomorphic forms to achieve
maximum acceptance. Negative reaction is more sensitive to motion than
appearance, so be particularly cognizant of jerky or unnatural movements when
animating anthropomorphic bodies and faces.
See also Anthropomorphic Form, Threat Detection, and Top-Down Lighting Bias.
1 The seminal work on the uncanny valley is
“Bukimi No Tani [The Uncanny Valley]” by
Masahiro Mori, Energy, 1970, vol. 7(4), p.
33–35.
2 See, for example, “Too Real for Comfort?
Uncanny Responses to Computer Generated
Faces” by Karl MacDorman, Robert Greena,
Chin-Chang Hoa, et al., Computers in Human
Behavior, May 2009, vol. 25(3), p. 695–710;
and “The Uncanny Valley: Effect of Realism on
the Impression of Artificial Human Faces” by
Jun’ichiro Seyama and Ruth Nagayama,
Presence, Aug. 2007, vol. 16(4), p. 337–351.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Uncanny Valley 243
Masahiro Mori’s classic graph plots
familiarity or appeal of an anthropo-
morphic form against its degree of
realism. The uncanny valley resides
to the right of the continuum, dipping
sharply just before the likeness of a
genuine healthy person. The manne-
quin images illustrate the benefits
of abstraction and total realism in
depicting human likenesses, as well
as the perils of the uncanny valley.
–
moving
humanoid robot
healthy person
bunraku puppet
prosthetic hand
corpse
zombie
stuffed animal
industrial robot
APPEAL
REALISM
UNCANNY VALLEY
50% 	100%
+
still
1
1
5
5
4
4
3
3
2
2

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Uncanny Valley** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Uncanny Valley để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Anthropomorphic Form, Threat Detection, and Top-Down Lighting Bias
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
