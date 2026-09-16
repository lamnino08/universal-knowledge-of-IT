---
name: "Five Hat Racks"
vi: "Năm chiếc giá treo mũ (Five Hat Racks)"
summary: "Five Hat Racks (Năm chiếc giá treo mũ (Five Hat Racks)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - perception
---

# Universal Design Principle: Five Hat Racks (Năm chiếc giá treo mũ (Five Hat Racks))

> **Tóm tắt cốt lõi (Summary)**: Five Hat Racks là một nguyên lý thiết kế then chốt thuộc nhóm **perception**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

There are five ways to organize information: category,
time, location, alphabet, and continuum.1
The organization of information is one of the most powerful factors influencing the
way people think about and interact with a design. The five hat racks principle
asserts that there are a limited number of organizational strategies, regardless of
the specific application: category, time, location, alphabet, and continuum.2
Category refers to organization by similarity or relatedness. Examples include
areas of study in a college catalog, and types of retail merchandise on a Web
site. Organize information by category when clusters of similarity exist within the
information, or when people will naturally seek out information by category (e.g., a
person desiring to purchase a stereo may seek a category for electronic appliances).
Time refers to organization by chronological sequence. Examples include historical
timelines and TV Guide schedules. Organize information by time when presenting
and comparing events over fixed durations, or when a time-based sequence is
involved (e.g., a step-by-step procedure).
Location refers to organization by geographical or spatial reference. Examples
include emergency exit maps and travel guides. Organize information by location
when orientation and wayfinding are important or when information is meaning-
fully related to the geography of a place (e.g., an historic site).
Alphabet refers to organization by alphabetical sequence. Examples include
dictionaries and encyclopedias. Organize information alphabetically, when
information is referential, when efficient nonlinear access to specific items is
required, or when no other organizing strategy is appropriate.
Continuum refers to organization by magnitude (e.g., highest to lowest, best to
worst). Examples include baseball batting averages and Internet search engine
results. Organize information by continuum when comparing things across a
common measure.
See also Advance Organizer, Consistency, and Framing.
1 The term hat racks is built on an analogy—
hats as information and racks as the ways to
organize information. Also known as five ways
of organizing information.
2 The seminal work on the five hat racks is
Information Anxiety by Richard Saul Wurman,
Bantam Books, 1990. Note that Wurman
changed the hat rack title of continuum to
hierarchy in a later edition of the book, which
permits the acronym LATCH. The original title
continuum is presented here, as the authors
believe it to be a more accurate description of
the category.
Five Hat Racks

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Canadian
National
Tower
Ostankino
Tower
Oriental
Pearl
Tower
Petronas
Towers
Sears
Tower
Menara
Kuala
Lumpur
Jin Mao
Building
World
Trade
Center
Tianjin
TV
Tower
Citic
Plaza
Canadian
National
Tower
Ostankino
Tower
Oriental
Pearl
Tower
Petronas
Towers
Sears
Tower
Jin Mao
Building
World
Trade
Center
Tianjin
TV
Tower
Citic
Plaza
Menara
Kuala
Lumpur
Canadian
National
Tower
Sears
Tower
World
Trade
Center
Ostankino
Tower 	Menara
Kuala
Lumpur
Petronas
Towers
Citic
Plaza
Jin Mao
Building
Tianjin
TV
Tower
Oriental
Pearl
Tower
Oriental
Pearl
Tower
Petronas
Towers
Menara
Kuala
Lumpur
Jin Mao
Building
Tianjin
TV
Tower
Citic
Plaza
Ostankino
Tower
World
Trade
Center
Sears
Tower
Canadian
National
Tower
1996	1974	1967 	1975 	1999	1991	1973 	1996	1995 	1998
Tianjin
TV
Tower
World
Trade
Center
Jin Mao
Building
Menara
Kuala
Lumpur
Sears
Tower
Petronas
Towers
Ostankino
Tower
Canadian
National
Tower
Citic
Plaza
Oriental
Pearl
Tower
1483'	1368'	1283' 	1381' 	1815'	1403'	1362' 	1535'	1450' 	1762'
The five hat racks are applied here
to the tallest structures in the world.
Although the same information is
presented in each case, the different
organizations dramatically influence
which aspects of the information
are emphasized.
Five Hat Racks 101
Alphabetical
Time
Location
Continuum
Category
Towers 	Buildings

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Five Hat Racks** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Five Hat Racks để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Advance Organizer, Consistency, and Framing
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
