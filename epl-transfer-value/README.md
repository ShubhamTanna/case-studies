# What Drives a Premier League Player's Transfer Value? (Regression Replication)

**Age, minutes played, goals and club rank explain most of what a Premier League player is worth. A 15-variable regression on 324 players from 2018–19 explains 68.4% of the variation in market value.**

## Question
Which player attributes (physical, performance and club) actually move a player's transfer value, and which don't?

## Source study
This project replicates Li, S. (2020), *Multiple regression model for predicting soccer player value in English Primer League*, The Frontiers of Society, Science and Technology, 2(15), 132–143. https://doi.org/10.25236/FSST.2020.021516

## Data
- 324 Premier League players, 2018–19 season (323 used after dropping one incomplete row)
- Sources: premierleague.com, Transfermarkt, FootyStats
- **Target:** player market value (log-transformed)
- **15 predictors:**
  - Physical: age, height, weight, position
  - Performance: average playing time, average appearance time, average goals, average assists, average clean sheets, penalty goals, penalty misses, red cards, yellow cards, player rank
  - Club: club rank

## Approach
1. Ran a Pearson correlation of each predictor against player value.
2. Fitted a multiple linear regression with all 15 predictors.
3. Checked model validity: F-test, multicollinearity (VIF) and autocorrelation (Durbin-Watson).

## Results
| Metric | Value |
|---|---|
| R² / Adjusted R² | 0.684 / 0.668 |
| F-statistic | 44.237 (p < 0.001) |
| Max VIF | 4.73 (below 5, so no serious multicollinearity) |
| Durbin-Watson | 1.82 (no meaningful autocorrelation) |

**Significant drivers (p < 0.001):**

| Driver | t-value | Direction |
|---|---|---|
| Age | −12.32 | Younger players are worth more |
| Club rank | −9.93 | Players at higher-ranked clubs are worth more |
| Average goals | 4.92 | More goals, more value |
| Average playing time | 3.89 | More minutes, more value |

- **Borderline:** average appearance time (p = 0.056).
- **Not significant:** height, weight, position, assists, clean sheets, penalties, cards and player rank.

## So what
For a club, value is mostly age, minutes, goals and where the player plays. Discipline and physical profile barely register. A scout looking for undervalued players should look for productive players with heavy minutes at lower-ranked clubs.

## Limitations
- One season only.
- Age and height are banded into categories rather than exact values.
- About a third of the variation in value is unexplained (likely reputation, contract length and commercial value).

## Tools
Python (pandas) for data preparation and regression; tables formatted in Google Sheets.

## My role
Solo research project (B.Tech CSBS, Semester 2, 2023). I replicated the published study's model and results. The original code and dataset were not retained.

## Folder contents
| Path | What it is |
|---|---|
| `EPL_Player_Value_Regression_Report.pdf` | The corrected report |
| `tables/table1_data_sample.png` | Sample of the 324-player dataset |
| `tables/table2_descriptive_stats.png` | Descriptive statistics |
| `tables/table3_correlations.png` | Correlation of each predictor with value |
| `tables/table4a_regression_coefficients.png` | Regression t-values, p-values and VIF |
| `tables/table4b_model_fit.png`, `table4c_model_fit_summary.png` | F, R², adjusted R², Durbin-Watson |
| `portfolio/` | The regression table as data, with sources (`facts.md`) |

---
**Shubham Tanna** · regression, hypothesis testing, sports analytics
<!-- SITE_LINK:work/epl-transfer-value -->
