# Aur Sunao: Building an Anonymous Listening App, from Idea to Pricing

**A six-person team designed a mental-health support app from scratch: the idea, user research, features, pricing plans and a clickable Figma prototype. Two years later I stress-tested our own pricing and found the flagship ₹499 plan cost ₹761 to deliver, then redesigned it to earn +₹154 per subscriber.**

Aur Sunao ("tell me more") is a concept app, designed but never launched. Its tagline is "Dil Se Dil Tak" (heart to heart).

**Team:** 6-person team project (B.Tech CSBS, Semester 5, 2024). The unit-economics review was added in 2026.

## The problem

We designed for people who are stressed and lonely but won't see a therapist because of the stigma and the time it takes. Our persona was a 23-year-old marketing executive who has just moved to a new city alone. She wants to talk things out without being judged, and without committing to therapy.

## What users told us

We ran an online survey (August 2024, 54 responses):

- **80%** prefer a human listener; only 2 of 54 prefer an AI.
- **78%** rate privacy 5 out of 5 in importance, yet only **17%** are comfortable sharing their feelings.
- **39%** need someone to talk to weekly or daily but find no one available.
- **11%** have ever used a platform like this.
- They want to talk: **67%** would use voice calls, **61%** text, **37%** video.

**Caveat:** this is a convenience sample, and 89% of respondents are aged 18–25. Treat the figures as directional.

## The product we designed

- **DilDost Calls (the core feature).** Anonymous calls with trained peer listeners, called DilDosts, who listen rather than diagnose. Users can pick a listener by gender and age.
- **Psychologist sessions.** 30-minute video sessions with licensed psychologists across India, filtered by experience, specialisation and rating.
- **Relaxing games.** Mandala art, jigsaw, sudoku and Tetris for quick stress relief between sessions.
- **AI chatbot.** A 24/7 helper for navigating the app, booking sessions and general questions.

## The business model

- **Basic plan, ₹499 a month:** 80 DilDost minutes, one 30-minute counsellor session, and unlimited chatbot and games.
- **FlexiFare, pay as you go:** ₹90 per 10 DilDost minutes and ₹450 per counsellor session.
- **Revenue split:** the listener or counsellor keeps 80% of what the user pays; the platform keeps 20%.

## The prototype

We sketched every screen on paper, then built 7 high-fidelity screens in Figma: sign-in, sign-up, home, top counsellors, chat, relaxing games and a DilDost call. The clickable prototype is at this [link](https://www.figma.com/proto/b5lymMQcj1m59Yzop4vkcD/AUR-SUNAO?node-id=317-769&t=QeVbKMk1CxHuieHL-1).

## Stress-testing our own pricing (2026)

I rebuilt the plan's economics in a live Excel model and found that the plan we designed lost money on every subscriber.

| ₹ per subscriber per month | Original Basic plan | Recommended plan (Option A) |
|---|---|---|
| Price | 499 | 499 |
| What's included | 80 DilDost min + one 30-min counsellor session + AI chatbot | 60 DilDost min; counsellor sold separately at ₹450; no AI chatbot |
| Cost to deliver | 761 | 357 |
| **Contribution** | **−262** | **+154** |
| Break-even | Never | **440 subscribers** |

- The ₹499 plan bundled ₹1,170 of pay-per-use value, a 57% discount. Every new subscriber added ₹262 to the monthly loss, so growth made things worse.
- Option A keeps the ₹499 price but changes what it includes:
  - 60 DilDost minutes instead of 80.
  - The counsellor session becomes pay-per-use at ₹450, earning ₹79 per session.
  - The AI chatbot is dropped. Only 2 of 54 survey respondents wanted an AI, and it carries clinical and liability risk.
- Option A stays profitable (+₹67 per subscriber) even if every subscriber uses all 60 minutes. Across the sensitivity grid (50–100% usage, 60–85% payout share), break-even ranges from 193 to 1,837 subscribers.

## What's inside

```
├── deck/Aur_Sunao_Pitch_Deck.pdf          31 slides: original pitch + 3 new slides (21–23): survey, unit economics, recommendation
├── deck/new_slide_21–23.png               the new slides as images
├── model/Aur_Sunao_Unit_Economics.xlsx    live model: Inputs, Unit Economics, Pay-per-use, Sensitivity, Scenarios, Notes
├── data/survey_responses_anonymised.csv   54 responses, names removed
├── portfolio/                         data behind the website charts, with sources (facts.md)
└── prototype/
    ├── screens/                           7 high-fidelity Figma screens
    └── sketches/                          the paper wireframes they came from
```

The interactive Figma prototype is at this [link](https://www.figma.com/proto/b5lymMQcj1m59Yzop4vkcD/AUR-SUNAO?node-id=317-769&t=QeVbKMk1CxHuieHL-1).

## Model assumptions (all editable in the Inputs sheet)

| Assumption | Value | Basis |
|---|---|---|
| Payout share to listeners and counsellors | 80% | The project's own revenue split, from its financial dashboard |
| Usage of included minutes and sessions | 80% | Assumption; see the Sensitivity sheet |
| Payment gateway fee | 2.36% | Razorpay standard pricing: 2% + 18% GST on the fee |
| Monthly fixed costs | ₹67,500 (₹70,000 with the AI chatbot) | Support salaries, marketing and hosting, from the project's FY25 financial snapshot |
| Option A: subscribers buying one paid counsellor session a month | 15% | Assumption |

**Methods:** problem framing, user survey, personas, feature design, pricing and business model, paper wireframes, prototyping in Figma, unit economics (contribution margin and break-even), sensitivity analysis.

---
Team of 6 (2024): idea, research, product, pricing plans, prototype · Shubham Tanna (2026): unit-economics model and redesign
<!-- SITE_LINK:work/aur-sunao -->
