# Facts: Aur Sunao

All unit-economics figures come from `model/Aur_Sunao_Unit_Economics.xlsx` (live formulas). Survey figures come from `data/survey_responses_anonymised.csv` (54 responses).

| Fact | Value | Source |
|---|---|---|
| Headline | Flagship ₹499 plan lost ₹262 per subscriber; redesigned plan earns +₹154 | Unit Economics sheet, row 18 |
| Cost to deliver | ₹761 original vs ₹357 recommended | Unit Economics sheet, row 22 |
| How +₹154 is built | ₹499 − ₹345.6 listener payouts − ₹11.8 gateway = +₹141.6, plus ₹11.9 from 15% of subscribers buying one ₹450 counsellor session at ₹79 margin | Unit Economics sheet, rows 9–18 |
| Break-even | 440 subscribers (₹67,500 ÷ ₹153.5) | Unit Economics sheet, row 21 |
| At 100% usage | still +₹67 per subscriber | Sensitivity sheet logic |
| Sensitivity range | break-even 193–1,837 subscribers across 50–100% usage and 60–85% payout share | Sensitivity sheet |
| Bundle discount | ₹1,170 of pay-per-use value sold for ₹499 (80 min × ₹9 + ₹450) | Inputs sheet |
| Survey | 54 respondents; 80% prefer a human listener, 2 of 54 prefer AI; 78% rate privacy 5/5; 39% need someone weekly or daily; 11% have used such a platform | survey CSV |
| Context | 6-person team project, Semester 5, 2024; unit-economics review added in 2026 | README |
| Contribution margin | −52.4% original vs 28.4% recommended | Unit Economics sheet, row 14 |
| Sensitivity grid | ₹37 to ₹351 contribution per subscriber across 50–100% usage and 60–85% payout share | Sensitivity sheet |
| Pay-per-use listener price | ₹90 per 10 minutes | Inputs sheet |
| AI chatbot maintenance (dropped in the redesign) | ₹2,500 a month | Inputs sheet |

## Key assumptions

80% payout share (the team's own split) · 80% usage of included minutes · Razorpay 2.36% gateway fee · 15% of subscribers buy one paid counsellor session a month · fixed costs from the team's FY25 snapshot.

## Caveats

- The survey is a convenience sample (89% aged 18–25), so treat its figures as directional.
- Numbers inside the prototype screens (dates, minutes, timers, IDs) are placeholder UI content, not data. The profile photo on the Home screen is blurred.

## Files

Deck: `deck/Aur_Sunao_Pitch_Deck.pdf` · Model: `model/Aur_Sunao_Unit_Economics.xlsx` · Survey: `data/survey_responses_anonymised.csv` · Screens: `prototype/screens/`
