# Facts: Aur Sunao

Aur Sunao is a concept app, designed but never launched. The idea, product, features, pricing plans and Figma prototype were built by a 6-person team (B.Tech CSBS, Semester 5, 2024). The unit-economics review was added in 2026.

Product facts come from the original pitch deck (`deck/Aur_Sunao_Pitch_Deck.pdf`, slides 1–20 and 24–31) and the prototype (`prototype/`). Unit-economics figures come from `model/Aur_Sunao_Unit_Economics.xlsx` (live formulas). Survey figures come from `data/survey_responses_anonymised.csv` (54 responses).

## The product

| Fact | Value | Source |
|---|---|---|
| Idea | Talk anonymously to a trained peer listener (a "DilDost") or book a video session with a licensed psychologist | deck slides 3, 10–13 |
| Tagline | "Dil Se Dil Tak" (heart to heart) | deck slide 1 |
| Vision | A world where every voice is heard and every story valued | deck slide 4 |
| Target user | Persona: 23-year-old marketing executive, recently moved to a new city alone; stressed and lonely but avoids therapy because of stigma and time | deck slides 6–8 |
| Core feature | DilDost Calls: anonymous calls with empathetic peer listeners; users can choose a listener by gender and age | deck slides 10–11 |
| Other features | Psychologist video sessions (30 min, filter by experience, specialisation and rating) · relaxing games (mandala art, jigsaw, sudoku, Tetris) · an AI chatbot for app help and support | deck slides 12–17; prototype screens |
| Features in the deck | 4 (DilDost Calls, psychologist sessions, relaxing games, AI chatbot) | deck slides 10–17 |
| Pricing plans | 2: Basic ₹499/month (80 DilDost minutes, one 30-min counsellor session, chatbot and games) and FlexiFare pay-per-use (₹90 per 10 DilDost minutes, ₹450 per counsellor session) | deck slides 18–20 |
| Revenue model | Listener or counsellor keeps 80% of what the user pays; the platform keeps 20% | model Inputs sheet (team's own revenue split) |
| Prototype | 7 high-fidelity Figma screens built from 5 paper sketches; clickable Figma prototype | `prototype/`; deck slide 31 |
| Survey | Online survey, 4–5 August 2024, 54 responses | survey CSV timestamps |

## What users told us (survey, 54 respondents)

| Fact | Value | Source |
|---|---|---|
| Prefer a human listener | 80% (43 of 54); 2 of 54 prefer AI; 17% no preference | survey CSV |
| Rate privacy 5 out of 5 | 78% | survey CSV |
| Comfortable sharing feelings (4–5 out of 5) | 17% | survey CSV |
| Want someone who both listens and advises | 80% | survey CSV |
| Need someone weekly or daily but find no one | 39% | survey CSV |
| Have ever used a platform like this | 11% | survey CSV |
| Prefer talking to express emotions | 91% (49 of 54 chose talking, alone or with another option) | survey CSV |
| Channel (could pick several) | voice 67%, text 61%, video 37% | survey CSV |

## The pricing review (2026)

| Fact | Value | Source |
|---|---|---|
| Headline | Flagship ₹499 plan lost ₹262 per subscriber; redesigned plan earns +₹154 | Unit Economics sheet, row 18 |
| Cost to deliver | ₹761 original vs ₹357 recommended | Unit Economics sheet, row 22 |
| How +₹154 is built | ₹499 − ₹345.6 listener payouts − ₹11.8 gateway = +₹141.6, plus ₹11.9 from 15% of subscribers buying one ₹450 counsellor session at ₹79 margin | Unit Economics sheet, rows 9–18 |
| Break-even | 440 subscribers (₹67,500 ÷ ₹153.5) | Unit Economics sheet, row 21 |
| At 100% usage | still +₹67 per subscriber | Sensitivity sheet logic |
| Sensitivity range | break-even 193–1,837 subscribers across 50–100% usage and 60–85% payout share | Sensitivity sheet |
| Sensitivity grid | ₹37 to ₹351 contribution per subscriber across 50–100% usage and 60–85% payout share | Sensitivity sheet |
| Contribution margin | −52.4% original vs 28.4% recommended | Unit Economics sheet, row 14 |
| Bundle discount | ₹1,170 of pay-per-use value sold for ₹499 (80 min × ₹9 + ₹450), a 57% discount | Inputs sheet |
| Pay-per-use listener price | ₹90 per 10 minutes | Inputs sheet |
| AI chatbot maintenance (dropped in the redesign) | ₹2,500 a month | Inputs sheet |
| Context | 6-person team project, Semester 5, 2024; unit-economics review added in 2026 | README |

## Key assumptions

80% payout share (the team's own split) · 80% usage of included minutes · Razorpay 2.36% gateway fee · 15% of subscribers buy one paid counsellor session a month · fixed costs from the team's FY25 snapshot.

## Caveats

- Aur Sunao is a concept: no app was launched, no listeners were recruited or trained, and there were no real users.
- The survey is a convenience sample (89% aged 18–25), so treat its figures as directional.
- Numbers inside the prototype screens (dates, minutes, timers, IDs) are placeholder UI content, not data. The profile photo on the Home screen is blurred.

## Files

Deck: `deck/Aur_Sunao_Pitch_Deck.pdf` · Model: `model/Aur_Sunao_Unit_Economics.xlsx` · Survey: `data/survey_responses_anonymised.csv` · Screens: `prototype/screens/` · Sketches: `prototype/sketches/`
