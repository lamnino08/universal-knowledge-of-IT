---
name: "Normal Distribution"
vi: "Phân phối chuẩn (Normal Distribution)"
summary: "Normal Distribution (Phân phối chuẩn (Normal Distribution)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - decision
---

# Universal Design Principle: Normal Distribution (Phân phối chuẩn (Normal Distribution))

> **Tóm tắt cốt lõi (Summary)**: Normal Distribution là một nguyên lý thiết kế then chốt thuộc nhóm **decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Normal Distribution
A term used to describe a set of data, that when plotted,
forms the shape of a symmetrical, bell-shaped curve.1
Normal distributions result when many independently measured values of a
variable are plotted. The resulting bell-shaped curve is symmetrical, rising from a
small number of cases at both extremes to a large number of cases in the middle.
Normal distributions are found everywhere—annual temperature averages,
stock market fluctuations, student test scores—and are thus commonly used to
determine the parameters of a design.
In a normal distribution, the average of the variable measured is also the most
common. As the variable deviates from this average, its frequency diminishes in
accordance with the area under the curve. However, it is a mistake to conclude
that the average is the preferred design parameter because it is the most
common. Generally, a range across the normal distribution must be considered
in defining design parameters, since variance between the average and the rest
of the population translates to the variance the design must accommodate. For
example, a shoe designed for the average of a population would fit only about 68
percent of the population.
Additionally, it is important to avoid trying to create something that is average in
all dimensions. A person average in one measure will not be average in other
measures. The probability that a person will match the average of their population
group in two measures is approximately 7 percent; this falls to less than 1 percent
for eight measures. The common belief that average people exist and are the
standard to which designers should design is called the “average person fallacy.”2
Where possible, create designs that will accommodate 98 percent of the
population; namely, the first to the 99th percentile. While design considerations
can be expanded to accommodate a larger portion of the population, generally,
the larger the audience accommodated, the greater the costs. Consideration of
the target population is key. When designing specifically for a narrow portion of
the population (e.g., airline seats that will accommodate 98 percent of American
males), it is crucial to obtain the appropriate measurement data for this very
specific group.
See also Convergence, Most Advanced Yet Acceptable, and Most Average Facial
Appearance Effect.

1 Also known as standard normal distribution,
Gaussian distribution, and bell curve.
2 Anthropometric data drawn from The Measure
of Man and Woman by Alvin R. Tilley and
Henry Dreyfuss Associates, The Whitney
Library of Design, 1993.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Normal Distribution 167
Top
of Head
Chin
Hips
Knee
Bottom
of Foot
Shoulders
Elbow
Wrist
Fingertip
male 	female 	male 	female 	male 	female
The measures of men and women are
normally distributed. The wide range
of measures across the distribution
illustrates the problem of simply
designing for an average group.
Note that no one man or woman is
represented by these measures—i.e.,
there is no average person in reality.
The normal distribution is represented
by a symmetric bell-shaped curve. The
four standard deviations represented
by below and above the average
reflect the normal percentages found
in the variability around the average.
Percentiles are indicated along the
bottom of the curve. Note that in a
normal distribution, approximately
68 percent of the population falls
within one standard deviation of the
average; approximately 95 percent
of the population falls within two
standard deviations of the average;
and approximately 99 percent of the
population falls within three standard
deviations of the average.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Normal Distribution** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Normal Distribution để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Convergence, Most Advanced Yet Acceptable, and Most Average Facial
Appearance Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
