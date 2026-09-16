---
name: "Personas"
vi: "Hồ sơ người dùng đại diện (Personas)"
summary: "Personas (Hồ sơ người dùng đại diện (Personas)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - decision
---

# Universal Design Principle: Personas (Hồ sơ người dùng đại diện (Personas))

> **Tóm tắt cốt lõi (Summary)**: Personas là một nguyên lý thiết kế then chốt thuộc nhóm **usability, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Personas
A technique that employs fictitious users to guide decision
making regarding features, interactions, and aesthetics.
The design that seeks to accommodate everybody generally accommodates
nobody well. For example, the percentage of visitors who actually buy products
on an e-commerce website is typically quite small relative to the total number of
visitors, but most website designs (and redesigns) fail to consider the differing
needs of buyers versus browsers — that is, they design for the average visitor, an
impersonal and homogenized construct derived from sources such as visitation
statistics, surveys, and usability testing. It is better to understand and perfectly
meet the needs of the critical few than to poorly meet the needs of many. It is this
specific problem that personas seek to address.1
Personas involve the creation of profiles for a small number of archetypal users,
each profile representing a composite of a subpopulation of users. Information
for the profiles is derived from user and stakeholder interviews, reviews of market
research and customer feedback, and statistics about how a product is used
when available. Done right, the number of personas is small, with typically no
more than three primary personas representing the primary target audience,
and up to four secondary personas when the needs of the user population are
highly stratified. Each persona is typically represented with a photograph, name,
description, and details about specific interests and relevant behaviors. It is often
useful for members of the design, development, and testing teams to role-play
different personas. This clarifies user needs and behaviors and is an effective
means of creating empathy for the user perspective. Personas not only make
the target audience more real to designers and engineers, they also ensure that
requirements are prioritized to specifically meet the needs of high-value users.
The use of personas in the design process is increasing in popularity, though
empirical evidence for the technique as compared to more traditional approaches
is lacking. The measurable merits of the approach are difficult to ascertain due
to the proprietary and relatively secretive nature of the methodology developed
by Cooper. The unfortunate result is an abundance of teachers, consultants,
and practitioners engaging in their own version or interpretation of personas.
Nevertheless, the anecdotal evidence for the general approach — especially its
user-sensitizing impact on designers and developers — is compelling.
Consider personas early in the design process to define and prioritize require-
ments. Keep persona profiles short, preferably one eye span, so that the
information can be easily consulted. Limit the number of primary personas to
three and secondary personas to four. Base personas on interviews and market
research — do not make them up or recycle personas from past projects. The time
required to research and develop personas is generally less than one month.
See also 80/20 Rule, Desire Line, Iteration, and Normal Distribution.
1 The seminal work on personas is The Inmates
Are Running the Asylum: Why High-Tech
Products Drive Us Crazy and How to Restore
the Sanity by Alan Cooper, SAMS, 1999. See
also The Persona Lifecycle: Keeping People in
Mind Throughout the Product Design by John
Pruitt and Tamara Adlin, Elsevier, 2006.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Personas 183
Three personas illustrating the varying
needs and behaviors of users for an
e-commerce website for toys. Amanda
is not generally a buyer, but she is an
influencer. She likes entertaining and
interactive websites. When she looks
for toys, she wants an easy way to
communicate (and lobby) her wish
list to her friends and family. Gloria is
the prototypical buyer. She is an over-
worked mom who worries about her
children being on the Internet. When
she visits the site, it is because her
kids are pestering her to buy some-
thing. Charles is an infrequent visitor.
He typically visits to buy his grandchil-
dren toys. He has no idea what toys
are “in” or what toys his grandchildren
already have. When he tries to buy, he
may need a lot of support.
Age
Occupation
Home Life
Education
Activities
Ultimate Goal
Web Usage
Web Competency
Frustrations
Frequent Sources of Information
Quote
AMANDA
7
Second grade student
Lives with her mother,
father, and younger
sister in the suburbs of
a large city.
In elementary school
Plays soccer, reads, and
takes ballet lessons;
saves her birthday
money and allowance to
spend at the mall.
Goal is to turn 10 so that
her parents will let her
baby-sit her cousins.
Uses the Web for school
projects and playing with
Webkinz.
Moderate competency
Gets frustrated because
her parents don’t always
buy her the cool stuff
that her friends have.
Friends, school, and
parents
“I can’t wait until I’m in
the fourth grade and get
a locker at school.”
66
Retired accountant
Lives with his wife
in the suburbs; has
four children and six
grandchildren.
Has an MBA
Likes to work in the
garden and drink wine.
Enjoys traveling with his
wife and investing in the
stock market.
Goal is to make sure
he and his wife have
enough money to enjoy
retirement and leave his
children an inheritance.
Uses the Web for email
and occasional research.
Also shares images and
videos of his grandkids.
Low competency
Gets frustrated when he
calls customer service
and can’t get a human
on the phone.
Cable network news and
Consumer Reports
“I worked hard my
whole life and now I am
enjoying my retirement
with my family.”
34
Part-time
office administrator
Lives with her husband
and two children in a
mid-sized city.
Has a bachelor degree
Enjoys crossword
puzzles and reading
mystery novels. Spends
a lot of time driving her
children to activities.
Goal is to make sure her
family is taken care of
and to find a little time
for herself each day.
Uses the Web for
shopping, news,
and communication.
Restricts the websites
that her children visit.
High competency
Gets frustrated by traffic
and waiting in line.
Feels like there is never
enough time.
Oprah, amazon.com,
and local TV news
“I love being a mom but
I often feel stressed and
need more balance in
my life.”
GLORIA 	CHARLES
WEB USE AND INFORMATION NEEDS
LIFESTYLE

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Personas** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Personas để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: 80/20 Rule, Desire Line, Iteration, and Normal Distribution
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
