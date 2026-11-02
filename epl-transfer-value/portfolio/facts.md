# Facts: EPL Transfer Value (regression replication)

| Fact | Value | Source |
|---|---|---|
| Headline | R² 0.684: 68.4% of market value explained by a 15-variable regression on 324 players | `tables/table4b_model_fit.png` |
| Significant drivers (p < 0.001) | age (t −12.32), club rank (−9.93), average goals (4.92), average playing time (3.89) | `tables/table4a_regression_coefficients.png` |
| Model checks | adjusted R² 0.668, F 44.237, max VIF 4.73, Durbin-Watson 1.82 | tables 4a and 4b |
| Source study | Li, S. (2020), doi:10.25236/FSST.2020.021516 | README |
| Context | Solo, Semester 2, 2023 | README |

## Caveats

- This is a replication of Li (2020), not original research.
- The saved results report t-values, p-values and VIF only. Coefficients, confidence intervals, RMSE and player-level predictions were not kept, and neither was the original code.

## Files

Report: `EPL_Player_Value_Regression_Report.pdf` · Tables: `tables/`
