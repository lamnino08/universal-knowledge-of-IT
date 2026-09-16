---
name: "Visuospatial Resonance"
vi: "Cộng hưởng thị giác không gian"
summary: "Visuospatial Resonance (Cộng hưởng thị giác không gian): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Visuospatial Resonance (Cộng hưởng thị giác không gian)

> **Tóm tắt cốt lõi (Summary)**: Visuospatial Resonance là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Visuospatial Resonance
A phenomenon in which an image achieves optimal
clarity due to resonance between the spatial frequency
of the image and the observer’s distance from the image.
Interpreting images is a process that involves interplay between visual informa-
tion received by the eyes and information stored in memory. The process begins
with the eyes first locating the primary lines, edges, and boundaries in an image,
pattern-matching these elements against elements in memory, and then proceeding
in this back-and-forth manner between eyes and memory at increasing levels of
detail until the interpretation is complete. The visibility of the lines, edges, and
boundaries in the image is a function of the spatial frequency of the image and
the distance to the observer. Images rendered at a high spatial frequency appear
as sharp outlines with little between-edge detail. High-spatial-frequency images
are easily interpreted up close, but are not visible from a distance. Images
rendered at a low spatial frequency appear as blurry images with little edge detail.
Low-spatial-frequency images are not visible up close, but are easily interpreted
from a distance. Images rendered at different spatial frequencies can be
combined to stunning effect, creating what are referred to as hybrid images.1
Perhaps the first known hybrid image effect is the elusive smile of Leonardo
da Vinci’s Mona Lisa. When observed up close and direct, Mona Lisa does not
appear to be smiling. However, when observed out of the corner of the eye or
at a distance, her subtle smile emerges. This effect is the result of two different
expressions rendered at different spatial scales — the nonsmiling mouth is rendered
at a high spatial frequency, which dominates direct proximal observation, and the
smiling mouth is rendered at a low spatial frequency, which dominates indirect
and nonproximal observation. Although da Vinci could not have understood the
modern science behind visuospatial resonance, it seems clear that he understood
the practical mechanism of the effect using shading — in the case of the Mona
Lisa, the elusive smile is achieved by applying shaded regions at the corners of
the mouth.2 This technique has been refined to create emotionally ambiguous
facial expressions, called gaze dependent facial expressions — that is, as an
observer gazes at an image, the image appears to morph.3
Consider visuospatial resonance as a means of increasing the propositional
density of static displays, increasing the interestingness of advertising posters and
billboards, masking sensitive text or image information, and creating emotionally
ambiguous facial expressions in artistic or photographic renderings of faces.
Although it is clear that visuospatial resonance can be achieved using hybrid
images with two images, it is not yet clear whether two images is the limit — that
is, whether visuospatial resonance is strictly a bimodal phenomenon (near and
far) limited to two-image hybrids, or a multimodal phenomenon potentially
accommodating any number of images.
See also Attractiveness Bias, Figure-Ground Relationship, and Law of Prägnanz.
1 The seminal work on visuospatial resonance
is “Masking in Visual Recognition: Effects of
Two-Dimensional Filtered Noise” by Leon D.
Harmon and Bela Julesz, Science, June 15,
1973, vol. 180(4091), p. 1194–1197; and
“From Blobs to Boundary Edges: Evidence
for Time- and Spatial-Scale-Dependent Scene
Recognition” by Philippe Schyns and Aude
Oliva, Psychological Science, 1994, vol. 5, p.
195–200. See also “Hybrid Images” by Aude
Oliva, Antonio Torralba, and Philippe Schyns,
ACM Transactions on Graphics, 2006, vol.
25(3), p. 527–532.
2 “Is It Warm? Is It Real? Or Just Low Spatial
Frequency?” by Margaret Livingstone, Science,
November 17, 2000, vol. 290(5495), p. 1299.
3 “Is That a Smile? Gaze Dependent Facial
Expressions” by Vidya Setlur and Bruce
Gooch, in NPAR ’04: Proceedings of the 3rd
International Symposium on Non-Photorealistic
Animation and Rendering, ACM Press, 2004,
p. 79–151.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

This hybrid image depicts two familiar
figures rendered at different spatial
frequencies. Up close, you see only
Albert Einstein, who is rendered at a
high spatial frequency. At a distance,
you see only Marilyn Monroe, who is
rendered at a low spatial frequency.
The distances at which the clarity of
each image is optimal are the points
of visuospatial resonance.
Visuospatial Resonance 253

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Visuospatial Resonance** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Visuospatial Resonance để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Attractiveness Bias, Figure-Ground Relationship, and Law of Prägnanz
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
