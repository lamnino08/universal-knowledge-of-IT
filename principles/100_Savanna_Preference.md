---
name: "Savanna Preference"
vi: "Sở thích thảo nguyên (Savanna Preference)"
summary: "Savanna Preference (Sở thích thảo nguyên (Savanna Preference)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - appeal
---

# Universal Design Principle: Savanna Preference (Sở thích thảo nguyên (Savanna Preference))

> **Tóm tắt cốt lõi (Summary)**: Savanna Preference là một nguyên lý thiết kế then chốt thuộc nhóm **appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

1 Also known as savanna hypothesis.
2 The seminal article on the savanna preference
is “Development of Visual Preference for
Natural Environments” by John D. Balling and
John H. Falkin, Environment and Behavior,
1982, vol. 14, p. 5–28.
3 See, for example, “The Biological Basis for
Human Values of Nature” by Stephen R.
Kellert, in The Biophilia Hypothesis by Stephen
R. Kellert and Edward O. Wilson (editors),
Island Press, 1993.

Savanna Preference
A tendency to prefer savanna-like environments to other
types of environments.1
People tend to prefer savanna-like environments—open areas, scattered trees,
water, and uniform grassiness—to other natural environments that are simple,
such as desert; dense, such as jungle; or complex, such as mountains. The
preference is based on the belief that early humans who lived on savannas
enjoyed a survival advantage over humans who lived in other environments. This
advantage ultimately resulted in the development of a genetic disposition favoring
savanna environments that manifests itself today. It may be no coincidence that
the parks, resorts, and golf courses of the world all resemble savannas—they
may reflect an unconscious preference for the look and feel of our ancestral,
east-African home.2
The characteristics of savannas that people prefer include depth, openness,
uniform grassy coverings, and scattered trees, as opposed to obstructed views,
disordered high complexity, and rough textures. The preference is found across
all age ranges and cultures, though it is strongest in children and grows weaker
with age. This finding is thought to corroborate the evolutionary origin of the
preference; i.e., humans are increasingly influenced by knowledge, culture, and
other environments as they grow older, interfering with innate preferences.
This causal explanation has been criticized as recent evidence suggests that
early humans lived in a variety of environments (e.g. closed-canopy woodlands),
but evidence for the existence of the preference is strong. For example, in an
experiment where people were presented with images of savannas, deciduous
forests, coniferous forests, rain forests, and desert environments, lush savannas
were consistently preferred over other choices as a place to live or visit. The
theory that the preference is related to the savanna’s perceived resource
richness is supported by the finding that the least preferred environment is the
arid desert landscape.3
People have a general landscape preference for savanna-like or parklike
environments that is independent of culture. Consider the savanna preference
in the design of landscapes, advertising, and any other design that involves the
creation or depiction of natural environments. The preference is strongest in young
children. Therefore, consider savanna-like environments in the design of settings
for children’s stories and play environments.
See also Archetypes, Biophilia Effect, Cathedral Effect, Hunter-Nurturer Fixations,
and Prospect-Refuge.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Savanna Preference 213
When presented with images of
environments such as these, people
across cultures generally prefer the
environments with unobstructed
views, uniform grassy coverings, and
scattered trees (left), as opposed to
obstructed views, high complexity,
and rough textures (right). This
preference is stronger in children
than in adults.
Though adults generally do not share
the fascination, the Teletubbies
(a children’s television series)
mesmerize children in more than 60
countries and 35 languages. Simple
stories played out by four baby-
faced creatures on a lush savanna
landscape equal excellent design for
young children.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Savanna Preference** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Savanna Preference để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Archetypes, Biophilia Effect, Cathedral Effect, Hunter-Nurturer Fixations,
and Prospect-Refuge
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
