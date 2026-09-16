---
name: "Signal-to-Noise Ratio"
vi: "Tỷ lệ tín hiệu trên nhiễu (SNR)"
summary: "Signal-to-Noise Ratio (Tỷ lệ tín hiệu trên nhiễu (SNR)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
  - learning
  - usability
  - appeal
---

# Universal Design Principle: Signal-to-Noise Ratio (Tỷ lệ tín hiệu trên nhiễu (SNR))

> **Tóm tắt cốt lõi (Summary)**: Signal-to-Noise Ratio là một nguyên lý thiết kế then chốt thuộc nhóm **perception, learning, usability, appeal**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Signal-to-Noise Ratio
The ratio of relevant to irrelevant information in a display. The
highest possible signal-to-noise ratio is desirable in design.
All communication involves the creation, transmission, and reception of
information. During each stage of this process, the form of the information—the
signal—is degraded, and extraneous information—noise—is added. Degradation
reduces the amount of useful information by altering its form. Noise reduces clarity
by diluting useful information with useless information. The clarity of information
can be understood as the ratio of remaining signal to added noise. For example, a
graph with no extraneous elements would have a high signal-to-noise ratio whereas,
a graph with many extraneous elements would have a low signal-to-noise ratio. The
goal of good design is to maximize signal and minimize noise, thereby producing a
high signal-to-noise ratio.1
Maximizing signal means clearly communicating information with minimal
degradation. Signal degradation occurs when information is presented inefficiently:
unclear writing, inappropriate graphs, or ambiguous icons and labels. Signal
clarity is improved through simple and concise presentation of information. Simple
designs incur minimal performance loads, enabling people to better focus on the
meaning of the information. Signal degradation is minimized through research
and careful decision-making. For example, failing to use the correct type of graph
to present a certain kind of data can fundamentally distort the meaning of the
information. It is therefore important to make good design decisions at the outset,
testing when necessary to verify design directions. Emphasizing key aspects of the
information can also reduce signal degradation—e.g., highlighting or redundantly
coding important elements in a design.
Minimizing noise means removing unnecessary elements, and minimizing the
expression of necessary elements. It is important to realize that every unnecessary
data item, graphic, line, or symbol steals attention away from relevant elements.
Such unnecessary elements should be avoided or else eliminated. Necessary
elements should be minimized to the degree possible without compromising
function. For example, the expression of lines in grids and tables should be
thinned, lightened, and possibly even removed. Every element in a design should
be expressed to the extent necessary, but not beyond the extent necessary.
Excess is noise.
Seek to maximize the signal-to-noise ratio in design. Increase signal by keeping
designs simple, and selecting design strategies carefully. Consider enhancing key
aspects of information through techniques like redundant coding and highlighting.
Use well-accepted standards and guidelines when available to leverage
conventions and promote consistent implementation. Minimize noise by removing
unnecessary elements, and minimizing the expression of elements.
See also Alignment, Horror Vacui, Layering, Performance Load, and Propositional
Density.

1 The seminal works on signal-to-noise ratio in
information design are “A Decision-Making
Theory of Visual Detection” by Wilson P.
Tanner Jr. and John A. Swets, Psychological
Review, 1954, vol. 61, p. 401–409; and Visual
Display of Quantitative Information by Edward
R. Tufte, Graphics Press, 1983.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

983
960
940
920
900
880
860
960
940
920
900
880
860
95 	96 	00	99	98	97 	1995 	1996 	2000	1999	1998	1997
869
884
919
939
981
1997
1998
1999
2000
2001
2.69
2.74
2.65
2.76
2.89
68.1
71.3
72.5
72.5
73.2
1997
1998
1999
2000
2001
2.69
2.74
2.65
2.76
2.89
68.1
71.3
72.5
72.5
73.2
Signal-to-Noise Ratio 225
SOYBEANS
PRODUCTION 	HARVESTED ACREAGE
Billions of Bushels 	Millions of Acres
Soybeans
Production 	Harvested Acreage
Billions of Bushels 	Millions of Acres
REGULAR ICE CREAM, U.S.
YEAR
Regular Ice Cream, U.S.
Millions of Gallons
Year
MILLIONS OF GALLONS
The signal-to-noise ratio of each of
these representations on the left is
improved by removing elements that
do not convey information, minimizing
the expression of remaining elements,
and highlighting essential information.
ALL OTHER 13.1
MOZZARELLA 30.6
OTHER AMERICAN 8.8
OTHER ITALIAN 8.7
SWISS 2.8
CHEDDAR 36.0
All Other 13.1 	Other
American
8.8
Swiss 2.8
	Mozzarella
30.6
Cheddar
36.0
1997
U.S. CHEESE
PRODUCTION
% BY TYPE
1997
U.S. Cheese
Production
% by Type
Other Italian 8.7

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Signal-to-Noise Ratio** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Signal-to-Noise Ratio để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Alignment, Horror Vacui, Layering, Performance Load, and Propositional
Density
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
