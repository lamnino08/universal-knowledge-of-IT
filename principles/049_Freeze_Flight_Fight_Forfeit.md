---
name: "Freeze-Flight-Fight-Forfeit"
vi: "Bốn phản ứng tự vệ (Freeze-Flight-Fight-Forfeit)"
summary: "Freeze-Flight-Fight-Forfeit (Bốn phản ứng tự vệ (Freeze-Flight-Fight-Forfeit)): Nguyên lý thiết kế cốt lõi giúp định hình giao diện và trải nghiệm tương tác trực quan, hiệu quả."
categories:
  - usability
  - decision
---

# Universal Design Principle: Freeze-Flight-Fight-Forfeit (Bốn phản ứng tự vệ (Freeze-Flight-Fight-Forfeit))

> **Tóm tắt cốt lõi (Summary)**: Freeze-Flight-Fight-Forfeit là một nguyên lý thiết kế then chốt thuộc nhóm **usability, decision**, giúp tối ưu hóa nhận thức người dùng, khả năng học hỏi và hiệu quả vận hành giao diện.

---

## 1. 📖 Tổng quan & Khái niệm (Concept Overview)

Freeze-Flight-Fight-Forfeit
The ordered sequence of responses to acute stress
in humans.1
When people are exposed to stressful or threatening situations, they respond in a
manner summarized by the catchy phrase, “fight or flight.” Less catchy but more
accurate is the contemporary construction, “freeze-flight-fight-forfeit,” which not
only describes the full set of responses, but also reflects the general sequence in
which they occur. The response set typically begins at stage one, and escalates
to subsequent stages as the level of threat increases:
If a threat is believed to be imminent, Freeze — a response characterized by
a state of hyperawareness and hypervigilance; purpose is to detect potential
threats (“stop, look, and listen” response).
If a threat is detected, take Flight — a response characterized by a state of
fear and panic; purpose is to escape from the threat (“run away” response).
If unable to escape the threat, Fight — a response characterized by a state of
desperation and aggression; purpose is to neutralize the threat (“fight for your
life” response).
If unable to neutralize the threat, Forfeit — a response characterized by
a state of tonic immobility and paralysis; purpose is to surrender to the
perceived threat (“playing dead” response).
These stages are innate responses that operate in all humans (and mammals
generally), though the triggers for each stage vary widely from person to person.
Depending on the strength of the threat stimulus, the response can skip stages.
For example, an unexpected explosion might immediately trigger a flight response
in some and a forfeit response in others. Training can alter the sensitivity to
triggers and the stage sequence. For example, soldiers are trained to freeze and
then fight and in some cases to never engage in flight or forfeit.
Consider freeze-flight-fight-forfeit in the design of systems that involve performance
under stress, such as the design of life-critical control systems (e.g., air traffic
control), emergency response plans and systems (e.g., emergency evacuation),
and emergency and self-defense training. Simplify tools, plans, and displays
appropriately in anticipation of diminished performance capabilities. Employ tools
and controls that require gross motor control only, and incorporate forgiveness to
prevent and minimize the effects of errors. Ensure the visibility of critical elements
to mitigate the effects of tunnel vision. In contexts where complex decision making
is required, avoid overusing alerts and alarms as they undermine concentration
and further burden cognitive functions.
See also Classical Conditioning, Defensible Space, and Threat Detection.
1 Also known as Fight or Flight and sympathetic
nervous system (SNS) reaction.
2 The seminal work on “fight or flight” is Bodily
Changes in Pain, Hunger, Fear and Rage:
An Account of Recent Research into the
Function of Emotional Excitement by Walter
Cannon, Appleton-Century-Crofts, 1929. The
updated construction — freeze-flight-fight-
forfeit — builds on proposals presented in The
Psychology of Fear and Stress by Jeffrey Alan
Gray, Cambridge University Press, 1988, and
“Does ‘Fight or Flight’ Need Updating?” by H.
Stefan Bracha, Tyler C. Ralston, Jennifer M.
Matsukawa, et al., Psychosomatics, October
2004, vol. 45, p. 448–449.

### Minh họa & Bối cảnh thực tế trong tài liệu gốc

Freeze-Flight-Fight-Forfeit 111
On January 15, 2009, US Airways
Flight 1549 suffers total engine failure
shortly after takeoff due to bird strike.
The plane is forced to ditch in the
Hudson River. The plane will sink
in 24 minutes. Passenger reaction
spans the freeze-flight-fight-forfeit
continuum, but the crew manages
this range of reactions through calm
and assertive leadership. As a result,
all 150 passengers and five crew
members survive the incident.
1
5
4
3
2
The crew directs passengers
to evacuate. In many cases,
however, their firm “Jump! Jump!
Jump!” commands overstimulate
the flight mode, and several
passengers jump into the frigid
waters of the Hudson River.
The cabin begins filling with
water from the rear. A panicked
passenger attempts to exit through
a rear emergency door. When
the aft crewmember intervenes,
the passenger’s fight mode is
activated. The passenger becomes
aggressive. The crew member
does not waver, and the passenger
eventually relents and moves
toward the front of the cabin.
Once everyone is believed to
have been evacuated from the
plane, the captain calmly walks
the length of the cabin twice to
make sure nobody is left behind.
This kind of cognitive override
of freeze-flight-fight-forfeit is
only attainable through years of
experience and extensive training.
The majority of passengers exit
through the emergency doors at
the wings where they congregate
as the plane sinks and rescue
vehicles approach, passengers go
into freeze mode; they fixate and
continuously reassess whether
to stay on the wings, swim to a
rescue vehicle, or attempt to swim
to shore.
The aisles quickly become
clogged with people as the water
level rises from the back. Despite
this visible and imminent threat,
a number of passengers remain
in their seats paralyzed with fear.
They are in forfeit mode. Crew
members snap them back to
flight mode by shouting at them
to climb over the seats toward the
front exits. The tactic is successful
and the passengers comply.

---

## 2. 🤖 Agent Instructions for UI/UX Design

Khi áp dụng nguyên lý **Freeze-Flight-Fight-Forfeit** vào thiết kế giao diện web/mobile:
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

> *"Áp dụng nguyên lý Freeze-Flight-Fight-Forfeit để tối ưu hóa nhận thức, giảm tải nhận thức và mang lại trải nghiệm tương tác liền mạch, chuyên nghiệp cho người dùng."*

---

## 6. 🔗 See Also & References

- **Các nguyên lý liên quan**: Classical Conditioning, Defensible Space, and Threat Detection
- **Tài liệu gốc**: *Universal Principles of Design* (William Lidwell, Kritina Holden, Jill Butler).
