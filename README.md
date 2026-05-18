# 🤖 Travel AI Tools

Hai công cụ AI miễn phí dành cho travel marketer — được build từ framework trong [travel-growth-playbook](https://github.com/thaolst/travel-growth-playbook).

Không cần cài đặt. Không lưu data. Chỉ cần Anthropic API key và trình duyệt.

![Last Commit](https://img.shields.io/github/last-commit/thaolst/travel-ai-tools?color=orange)
![License](https://img.shields.io/github/license/thaolst/travel-ai-tools)
![Stars](https://img.shields.io/github/stars/thaolst/travel-ai-tools?style=social)
![Free](https://img.shields.io/badge/free-forever-brightgreen)
![No Data Stored](https://img.shields.io/badge/data-none%20stored-lightgrey)
![Powered by Claude](https://img.shields.io/badge/powered%20by-Claude%20AI-orange)
![Language](https://img.shields.io/badge/language-VI%20%2B%20EN-blue)

🔗 **[→ Dùng thử tại thaolst.github.io/travel-ai-tools](https://thaolst.github.io/travel-ai-tools)**

---

## 🛠️ Hai công cụ

### 🧭 Campaign Brief Generator
[`campaign-brief-generator.html`](./campaign-brief-generator.html) · [→ Dùng thử](https://thaolst.github.io/travel-ai-tools/campaign-brief-generator.html)

Chọn segment, vertical, mùa, và goal. Nhận full campaign brief trong 2 phút, bao gồm:

- Campaign objective rõ ràng và đo được
- Key insight về segment trong giai đoạn đó
- Message angles (emotional, functional, urgency)
- Promotion mechanic cụ thể — không vague
- Channel plan theo thứ tự ưu tiên
- KPIs với target thực tế cho thị trường Vietnam
- Những điều cần tránh

<details>
<summary><b>📸 Xem ví dụ output — Explorer × Tết × Airline + Bundle</b></summary>

```
## Campaign Objective
Tăng 25% repeat booking rate của Explorer segment trong giai đoạn Tết 
trong 6 tuần, đo bằng tỉ lệ users mua bundle (flight + hotel) sau khi 
click campaign.

## Target Audience
Explorer segment — travelers 25-35, đi 3-4 chặng/năm, đã từng book 
airline nhưng chưa bao giờ mua bundle. Tết họ cần về quê hoặc đi chơi 
dài ngày, và đang stress vì giá vé cao + thủ tục phức tạp.

## Key Insight
Explorer ghét cảm giác bị "sale" nhưng thích "chiến lược" — họ sẽ 
mua nếu thấy bundle là cách thông minh để tiết kiệm, không phải là 
khuyến mãi rẻ tiền.

## Campaign Message
Core: "Về Tết thông minh hơn — một lần book, cả chặng đường."

Execution angles:
- Emotional: "Để dành năng lượng cho gia đình, không phải xếp lịch"
- Functional: "Bundle flight + hotel, tiết kiệm đến 30% so với book rời"
- Urgency: "Giá Tết sẽ tăng trong 48h — lock ngay với chỉ 200k trước"

## Promotion Mechanic
Exclusive bundle offer: flight + hotel combo, giảm 25-30% so với 
book rời, max discount 500k VND, valid 7 ngày sau khi nhận offer, 
chỉ cho users đã từng bay nhưng chưa mua bundle.

Mechanic phù hợp vì: Explorer không reactive với discount thông 
thường — bundle là upsell hợp lý dựa trên behavior (họ đã bay) và 
nhu cầu Tết (cả nhà đi, cần chỗ ở).

## Channel Plan
1. Push notification — day 1: "Your Tết bundle is ready" 
    (personalized với destination họ đã search)
2. Email — day 2: full bundle breakdown + savings calculator
3. In-app banner — homepage + search results page
4. Zalo OA — day 3: reminder + social proof ("2,000+ travelers đã 
    book bundle cho Tết này")
5. Retargeting (FB/IG) — users đã click nhưng chưa book

## KPIs
- Primary: Repeat bundle booking rate → target 12% of targeted cohort
- Efficiency: Bundle CAC → target < 35k VND per booking
- Quality: Bundle NPS → target > 60 (đo 7 ngày sau trip)

## Watch Out For
- Tính thanh khoản thấp của bundle so với book rời — nếu bundle quá 
    rigid (non-refundable, fixed dates), Explorer sẽ drop. 
    Cần ít nhất 1 lần free reschedule.
- Tết là peak season, inventory có hạn — đừng chạy campaign quá 
    rộng nếu supply không đủ. Giới hạn booking window.
- Over-discounting — giảm quá 30% làm mất giá trị brand. 
    25% là sweet spot cho bundle Tết.
```
</details>

### 🔬 Retention Cohort Diagnose
[`retention-diagnose.html`](./retention-diagnose.html) · [→ Dùng thử](https://thaolst.github.io/travel-ai-tools/retention-diagnose.html)

Mô tả cohort — số booking, first booking, last booking, những gì đã thử. Nhận:

- Risk level: High / Medium / Low
- Root cause analysis cụ thể với travel behavior
- Top 3 churn signals
- 90-day playbook với action cụ thể theo từng phase
- Những gì không nên làm
- Success metrics

<details>
<summary><b>📸 Xem ví dụ output — Cohort 1-booking, Bus user, 6 tháng chưa quay lại</b></summary>

```
## RISK LEVEL
HIGH — Một booking duy nhất, cách đây 6-12 tháng, không có 
tương tác nào sau đó. Đây là single-booking cohort — nhóm 
dễ mất nhất trên travel platform.

## ROOT CAUSE ANALYSIS
Bus vertical có natural frequency rất thấp (2-3 chuyến/năm với 
người dùng thường xuyên). Với người dùng chỉ có 1 booking 6-12 
tháng trước, rủi ro cao nhất là họ đã: (1) chuyển sang đối thủ 
vì giá hoặc UX, (2) chỉ có nhu cầu đặc biệt 1 lần (về quê 
dịp lễ), hoặc (3) không biết platform còn các dịch vụ khác 
như hotel/train.

Thực tế, bus user single-booking khác airline một-booking — bus 
thường là chuyến ngắn ngày, giá trị thấp, nên activation 
cost thấp hơn. Nhưng retention cost lại cao hơn vì trung thành 
với thương hiệu bus truyền thống là chính (xe nhà, dòng họ).

Điểm mấu chốt: 6 tháng là critical gap. Với bus, nếu user 
không quay lại trong 90 ngày sau first booking, khả năng 
quay lại giảm 60%. Ở tháng thứ 6, họ gần như đã hình thành 
thói quen mới với đối thủ.

## TOP 3 CHURN SIGNALS
1. Single booking gap > 6 tháng — Trên bus vertical, đây là 
   dấu hiệu rõ ràng nhất. Không phải natural dormant — họ 
   đã chọn kênh khác.

2. Không có cross-vertical signal — Nếu họ book bus mà 
   không hề search hotel/train/airline, user này có trip 
   intent rất hẹp và dễ mất.

3. Không reactive với reminder — Nếu bạn đã gửi voucher 
   discount 30% và họ (1) không mở hoặc (2) không click, 
   đây là confirmation cuối cùng.

## 90-DAY PLAYBOOK

Phase 1: Re-engagement (Day 1-30)
- Day 1: Gửi push + email "Chúng tôi nhớ bạn" — không phải 
    voucher, mà là personalised recap: route họ đã đi + gợi ý 
    route tương tự với giá hiện tại.
- Day 7: Nếu không react — SMS voucher 50k cho bus route bất 
    kỳ (activation cost thấp, đủ để thử lại).
- Day 14: Zalo OA — share route inspiration cho dịp lễ sắp 
    tới (30/4 hoặc Tết), có CTA book bus + hotel.

Phase 2: Cross-sell activation (Day 31-60)
- Day 35: Giới thiệu hotel vertical — "Bạn đã đi bus đến 
    Đà Lạt? Khám phá hotel deal cạnh bến xe, chỉ từ 299k."
- Day 45: Bundle deal bus + hotel, exclusive 15% off, 
    7-day expiry. Đây là upsell có behavior justification.

Phase 3: Loyalty seeding (Day 61-90)
- Day 70: Mời tham gia loyalty tier nhẹ — "Chỉ cần 1 chuyến 
    nữa trong 30 ngày, bạn sẽ được free bus ticket cho tháng sau."
- Day 90: Nếu vẫn inactive — move cohort sang win-back 
    campaign riêng với higher incentive.

## WHAT NOT TO DO
- Đừng gửi discount generic — user này đã thấy và ignore. 
    Cần thay đổi format hoàn toàn.
- Đừng multi-channel spam — nếu push không react, đừng 
    đẩy email ngay lập tức. Spacing giữa các touchpoint 
    trong phase 1 là 7 ngày.

## SUCCESS METRICS
- Phase 1: Re-activation rate → target 8% (tỉ lệ user quay 
    lại book trong 30 ngày)
- Phase 2: Cross-sell rate → target 12% của cohort đã reactivate
- Phase 3: Repeat rate trong 90 days → target 20% (2+ bookings)
```
</details>

---

> ⚡ Cả 2 tool cho output ngay sau ~10-15 giây. Không cần tài khoản, không cần đăng ký — chỉ cần API key.

---

## 🔑 Cách dùng

Cả hai tool cần Anthropic API key. Lấy key miễn phí tại [console.anthropic.com](https://console.anthropic.com).

API key chỉ tồn tại trong browser trong phiên dùng đó. Không được lưu, không gửi đến đâu ngoài API của Anthropic.

Không muốn dùng API key? Mỗi tool đều có **Prompt Chain Backup** — copy prompt ra dùng trực tiếp trong Claude.ai hoặc ChatGPT, không cần trả thêm tiền.

## 📁 File structure

```
travel-ai-tools/
├── README.md
├── index.html                      ← Landing page
├── campaign-brief-generator.html   ← Tool 1
└── retention-diagnose.html         ← Tool 2
```

## 🔗 Liên quan

Đây là phần ứng dụng AI của [travel-growth-playbook](https://github.com/thaolst/travel-growth-playbook) — repo chứa framework và playbook đầy đủ về growth marketing trong travel vertical.

## 👤 Tác giả

Growth Marketing Manager với kinh nghiệm launch và scale travel platform tại Việt Nam, covering airline, bus, train, hotel, và experience verticals.
🔗 [Facebook](https://www.facebook.com/LeSongTienThao) · [LinkedIn](https://linkedin.com/in/thaolst) · [X](https://x.com/thaolst)

---

# 🤖 Travel AI Tools

Two free AI tools for travel marketers — built on the frameworks in [travel-growth-playbook](https://github.com/thaolst/travel-growth-playbook).

No installation. No data stored. Just an Anthropic API key and a browser.

🔗 **[→ Try at thaolst.github.io/travel-ai-tools](https://thaolst.github.io/travel-ai-tools)**

---

## 🛠️ Two Tools

### 🧭 Campaign Brief Generator
[`campaign-brief-generator.html`](./campaign-brief-generator.html) · [→ Try it](https://thaolst.github.io/travel-ai-tools/campaign-brief-generator.html)

Select segment, vertical, season, and goal. Get a full campaign brief in 2 minutes, including:

- A clear, measurable campaign objective
- Key insight about the segment in that period
- Message angles (emotional, functional, urgency)
- Specific promotion mechanic — not vague
- Prioritized channel plan
- KPIs with realistic targets for the Vietnam travel market
- What to watch out for

<details>
<summary><b>📸 See sample output — Explorer × Tết × Airline + Bundle</b></summary>

```
## Campaign Objective
Increase Explorer segment's repeat booking rate by 25% during the 
Tết period over 6 weeks, measured by bundle (flight + hotel) 
purchase rate after campaign click.

## Target Audience
Explorer segment — ages 25-35, 3-4 trips/year, has booked airline 
but never bought a bundle. During Tết they need to travel home or 
take extended holidays, and are stressed about peak pricing and 
complex logistics.

## Key Insight
Explorers hate being "sold to" but love "strategy" — they'll buy 
a bundle if they see it as a smart way to save, not a cheap promotion.

## Campaign Message
Core: "Travel smarter this Tết — one booking, one trip."

Execution angles:
- Emotional: "Save your energy for family, not for logistics"
- Functional: "Flight + hotel bundle, save up to 30% vs. booking separately"
- Urgency: "Tết prices will rise in 48h — lock yours with just 200k deposit"

## Promotion Mechanic
Exclusive bundle offer: flight + hotel combo, 25-30% off vs. 
separate bookings, max discount 500k VND, valid 7 days after 
receiving offer, only for users who've flown but never purchased a bundle.

Why this fits: Explorers don't react to standard discounts — 
bundles are a logical upsell based on their behavior (already flying) 
and Tết need (family trip requires accommodation).

## Channel Plan
1. Push notification — day 1: "Your Tết bundle is ready" 
    (personalized to their searched destination)
2. Email — day 2: full bundle breakdown + savings calculator
3. In-app banner — homepage + search results page
4. Zalo OA — day 3: reminder + social proof ("2,000+ travelers 
    have booked bundles for Tết")
5. Retargeting (FB/IG) — users who clicked but didn't book

## KPIs
- Primary: Repeat bundle booking rate → target 12% of cohort
- Efficiency: Bundle CAC → target < 35k VND per booking
- Quality: Bundle NPS → target > 60 (measured 7 days post-trip)

## Watch Out For
- Bundle liquidity is lower than separate bookings — if bundles are 
    too rigid (non-refundable, fixed dates), Explorers will drop off. 
    Include at least 1 free reschedule.
- Tết is peak season with limited inventory — don't scale the 
    campaign too broadly if supply is constrained. Cap the booking window.
- Over-discounting hurts brand value. 25% off is the sweet spot 
    for Tết bundles. Anything above 30% devalues the offer.
```
</details>

### 🔬 Retention Cohort Diagnose
[`retention-diagnose.html`](./retention-diagnose.html) · [→ Try it](https://thaolst.github.io/travel-ai-tools/retention-diagnose.html)

Describe a cohort — booking count, first booking, last booking, what you've tried. Get:

- Risk level: High / Medium / Low
- Root cause analysis specific to travel behavior
- Top 3 churn signals
- 90-day playbook with specific actions per phase
- What not to do
- Success metrics

<details>
<summary><b>📸 See sample output — 1-booking cohort, Bus user, inactive 6+ months</b></summary>

```
## RISK LEVEL
HIGH — Single booking, 6-12 months ago, zero interaction since. 
This is a classic single-booking cohort — the most vulnerable 
group on any travel platform.

## ROOT CAUSE ANALYSIS
Bus vertical has naturally low frequency (2-3 trips/year for 
regular users). For a user with only 1 booking 6-12 months ago, 
the highest risks are: (1) they've switched to a competitor 
for price or UX reasons, (2) it was a one-off need (holiday 
travel home), or (3) they don't know the platform offers 
other services like hotel/train.

A single bus booking differs from a single airline booking — 
bus trips are shorter and lower value, so activation cost is 
lower. But retention cost is higher because loyalty to 
traditional bus brands (family-run, word-of-mouth) is strong.

The critical insight: 6 months is the danger zone for bus users. 
If they don't return within 90 days of first booking, 
return probability drops 60%. By month 6, they've likely 
formed a new habit with a competitor.

## TOP 3 CHURN SIGNALS
1. Single booking with 6+ month gap — On bus vertical, this is 
   the clearest signal. Not natural dormancy — they've 
   chosen another channel.

2. No cross-vertical signal — If they booked bus but never 
   searched hotel/train/airline, this user has very narrow 
   trip intent and is easy to lose.

3. No reaction to reminders — If you sent a 30% discount 
   voucher with (1) no open or (2) no click, this is final 
   confirmation they're gone.

## 90-DAY PLAYBOOK

Phase 1: Re-engagement (Day 1-30)
- Day 1: Push + email "We miss you" — not a voucher, but a 
    personalized recap: their past route + similar route 
    suggestions with current pricing.
- Day 7: If no reaction — SMS voucher 50k off any bus route 
    (low activation cost, enough for a trial).
- Day 14: Zalo OA — route inspiration for next upcoming holiday 
    (30/4 or Tết), with bus + hotel CTA.

Phase 2: Cross-sell activation (Day 31-60)
- Day 35: Introduce hotel vertical — "You took the bus to 
    Da Lat? Check out hotel deals near the bus station, from 299k."
- Day 45: Bundle deal bus + hotel, exclusive 15% off, 
    7-day expiry. Behavior-justified upsell.

Phase 3: Loyalty seeding (Day 61-90)
- Day 70: Light loyalty tier invite — "Book once more in 
    30 days, get a free bus ticket next month."
- Day 90: Still inactive? Move cohort to dedicated win-back 
    campaign with higher incentive.

## WHAT NOT TO DO
- Don't send generic discounts — this user has already seen 
    and ignored them. Need a completely different format.
- Don't multi-channel spam — if push didn't react, don't 
    immediately send email. Spacing between phase 1 
    touchpoints should be 7 days minimum.

## SUCCESS METRICS
- Phase 1: Re-activation rate → target 8% (users who return 
    and book within 30 days)
- Phase 2: Cross-sell rate → target 12% of reactivated cohort
- Phase 3: Repeat rate within 90 days → target 20% (2+ bookings)
```
</details>

---

> ⚡ Both tools return output in ~10-15 seconds. No account, no signup — just an API key.

---

## 🔑 How to Use

Both tools require an Anthropic API key. Get one free at [console.anthropic.com](https://console.anthropic.com).

The API key only lives in your browser during that session. It's never stored and is sent only to Anthropic's API.

No API key? Both tools include a **Prompt Chain Backup** — copy the prompt and use it directly in Claude.ai or ChatGPT at no extra cost.

## 📁 File Structure

```
travel-ai-tools/
├── README.md
├── index.html                      ← Landing page
├── campaign-brief-generator.html   ← Tool 1
└── retention-diagnose.html         ← Tool 2
```

## 🔗 Related

This is the AI application layer of [travel-growth-playbook](https://github.com/thaolst/travel-growth-playbook) — the full framework and playbook repo for travel growth marketing.

## 👤 Author

Growth Marketing Manager with experience launching and scaling a multi-modal travel platform in Vietnam, covering airline, bus, train, hotel, and experience verticals. Building at the intersection of **Growth Marketing × AI**.

🔗 [Facebook](https://www.facebook.com/LeSongTienThao) · [LinkedIn](https://linkedin.com/in/thaolst) · [X](https://x.com/thaolst)
