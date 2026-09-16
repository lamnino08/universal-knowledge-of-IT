---
name: "Face-ism Ratio"
vi: "Tỷ lệ khuôn mặt trên cơ thể"
summary: "Face-ism Ratio (Tỷ lệ khuôn mặt trên cơ thể): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - appeal
---

# Universal Design Principle: Face-ism Ratio (Tỷ lệ khuôn mặt trên cơ thể)

> **Tóm tắt cốt lõi (Summary)**: Face-ism Ratio là một nguyên lý thiết kế then chốt thuộc nhóm **perception, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

The ratio of face to body in an image that influences the
way the person in the image is perceived.1
Images depicting a person with a high face-ism ratio—the face takes up most of
the image—focus attention on the person’s intellectual and personality attributes.
Images depicting a person in a low face-ism ratio—the body takes up most of the
image—focus attention on the physical and sensual attributes of the person. The
face-ism ratio is calculated by dividing the distance from the top of the head to the
bottom of the chin (head height) by the distance from the top of the head to the
lowest visible part of the body (total visible height). An image without a face would
have a face-ism ratio of 0.00, and an image with only a face would have a face-
ism ratio of 1.00. Irrespective of gender, people rate individuals in high face-ism
images as being more intelligent, dominant, and ambitious than individuals in low
face-ism images.
The term face-ism originated from research on gender bias in the media. It
was found that images of men in magazines, movies, and other media have
significantly higher face-ism ratios than images of women. This appears true
across most cultures, and is thought to reflect gender-stereotypical beliefs
regarding the characteristics of men and women. While there is little consensus
as to why this is the case, it is likely the result of unconscious processes resulting
from a mix of biological and cultural factors. In one experiment, for example, male
and female college students were randomly assigned a task to draw either a man
or a woman. The students were told they would be evaluated on their drawing
skills, and were given no additional instructions. Both genders drew men with
prominent and detailed faces, and drew women with full bodies and minimally
detailed faces.2
Consider face-ism in the representation of people in photographs and drawings.
When the design objective requires more thoughtful interpretations or associations,
use images with high face-ism ratios. When the design objective requires more
ornamental interpretations or associations, use images with low-face-ism ratios.
Note that the interpretations of the images will be the same irrespective of the
subject’s or viewer’s gender.
See also Attractiveness Bias, Baby-Face Bias, Classical Conditioning, Framing,
and Waist-to-Hip Ratio.
1 The term face-ism is used by some
researchers to refer to the tendency of the
media to represent men in high face-ism
images, and women in low face-ism images—
also referred to as body-ism.
2 The seminal work on face-ism is “Face-ism”
by Dane Archer, Debra D. Kimes, and Michael
Barrios, Psychology Today, 1978, p. 65–66;
and “Face-ism: 5 Studies of Sex-Differences
in Facial Prominence” by Dane Archer, Bonita
Iritani, Debra D. Kimes, and Michael Barrios,
Journal of Personality and Social Psychology,
1983, vol. 45, p. 725–735.
Face-ism Ratio

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Face-ism Ratio 89
The effect of face-ism is evident in
these photographs. The high face-ism
photograph emphasizes more cerebral
or personality-related attributes like
intelligence and ambition. The lower
face-ism photographs emphasize more
physical attributes like sensuality and
physical attractiveness.
Face-ism Ratio = .96 	Face-ism Ratio = .55 	Face-ism Ratio = .37

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Face-ism Ratio** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Face-ism Ratio để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Attractiveness Bias, Baby-Face Bias, Classical Conditioning, Framing,
and Waist-to-Hip Ratio
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
