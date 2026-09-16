---
name: "Mnemonic Device"
vi: "Kỹ thuật ghi nhớ (Mnemonic Device)"
summary: "Mnemonic Device (Kỹ thuật ghi nhớ (Mnemonic Device)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - learning
---

# Universal Design Principle: Mnemonic Device (Kỹ thuật ghi nhớ (Mnemonic Device))

> **Tóm tắt cốt lõi (Summary)**: Mnemonic Device là một nguyên lý thiết kế then chốt thuộc nhóm **learning**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Mnemonic Device
A method of reorganizing information to make the
information easier to remember.
Mnemonic devices are used to reorganize information so that the information
is simpler and more meaningful and, therefore, more easily remembered. They
involve the use of imagery or words in specific ways to link unfamiliar information
to familiar information that resides in memory. Mnemonic devices that involve
imagery are strongest when they are vivid, peculiar, and exaggerated in size or
quantity. Mnemonic devices that involve words are strongest when the words are
familiar and clearly related. Mnemonic devices are useful for remembering names
of new things, large amounts of rote information, and sequences of events or
procedures. A few examples of mnemonic devices include:1
First-Letter—The first letter of items to be recalled are used to form the first
letters in a meaningful phrase, or combined to form an acronym. For example,
Please Excuse My Dear Aunt Sally to assist in the recall of the arithmetic order of
operations: Parentheses, Exponents, Multiplication, Division, Addition, Subtraction;
or AIDS as a simple means of referring to and remembering Acquired Immune
Deficiency Syndrome.
Keyword—A word that is similar to, or a subset of, a word or phrase that is linked
to a familiar bridging image to aid in recall. For example, the insurance company
AFLAC makes its company name more memorable by reinforcing the similarity
of the pronunciation of AFLAC and the quack of the duck. The duck in the
advertising is the bridging image.
Rhyme—One or more words in a phrase are linked to other words in the phrase
through rhyming schemes to aid in recall. For example, red touches yellow kill a
fellow is a popular mnemonic to distinguish the venomous coral snake from the
nonvenomous king snake.
Feature-Name—A word that is related to one or more features of something that
is linked to a familiar bridging image to aid in recall. For example, the rounded
shape of the Volkswagen Beetle is a key feature of its biological namesake, which
serves as the bridging image.
Consider mnemonic devices when developing corporate and product identities,
slogans and logos for advertising campaigns, instructional materials dealing with
rote information and complex procedures, and other contexts in which ease
of recall is critical to success. Use vivid and concrete imagery and words that
leverage familiar and related concepts.
See also Chunking, Serial Position Effects, and von Restorff Effect.

1 The seminal contemporary work on
mnemonics is The Art of Memory by Frances
A. Yates, University of Chicago Press, 1974.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Clever use of mnemonic devices can
dramatically influence recall. These
logos employ various combinations
of mnemonic devices to make them
more memorable.
Mnemonic Device 159

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Mnemonic Device** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Mnemonic Device để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Chunking, Serial Position Effects, and von Restorff Effect
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
