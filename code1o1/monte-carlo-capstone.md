# Monte Carlo Portfolio Simulator

*The capstone project of Code1o1's Python in Finance course (40 one-hour 1:1 sessions, taught to a first-year BBA student).*

This interactive Streamlit dashboard answers one question: **"If I invest in this mix of stocks, what range of outcomes could I realistically expect?"**

The user picks any combination of 8 NSE-listed assets (Infosys, TCS, HDFC Bank, Reliance, ITC, Sun Pharma, Maruti, Gold BeES), sets the amount and the time horizon, and the app simulates thousands of possible futures. The simulation uses each stock's real price history, including how the stocks move together.

## What it shows

- A **fan chart** of portfolio value over time: the median path and the 5th–95th percentile band.
- The **distribution of final values**, with the amount invested, the median and the 5th percentile marked.
- **Risk numbers:** median outcome, 90% range, probability of profit, Value at Risk (95%).
- The **diversification effect:** a correlation heatmap, and the portfolio's volatility compared with what it would be if every stock moved in lockstep.
- A plain-English **methodology and limitations** section.

## How the model works

1. Download five years of adjusted daily prices (Yahoo Finance via `yfinance`) and convert them to daily returns.
2. Estimate each stock's mean return and the covariance between every pair of stocks.
3. Draw correlated daily returns with `numpy.random.Generator.multivariate_normal`, so the simulated stocks keep their real-life relationships.
4. Combine the returns using the portfolio weights and compound them into thousands of price paths.
5. Summarise the outcomes with percentiles, probability of profit and Value at Risk.

**Limitations, stated in the app:**
- Returns are assumed to be normally distributed, so real fat-tailed crashes are understated.
- Means and correlations are held constant at their five-year values.
- Weights are rebalanced daily.
- No fees, taxes or inflation.

## How I designed it as a teaching project

- **A working version and a student version.** I built a complete working version first, with a 36-test automated suite. A script (`tools/build_scaffold.py`) then removes the marked solution blocks to produce the student's version. In that version, the tests fail until she writes each function herself, so she gets instant, objective feedback.
- **Six sessions, each with one goal:**
  1. A single simulated price path.
  2. Thousands of paths and the fan chart.
  3. Reading the results, plus multi-stock returns and correlation.
  4. The portfolio simulation.
  5. Wiring up the app in GitHub Codespaces.
  6. Methodology, README, deployment and a spoken walkthrough.
- **Honest scope cuts.** Sharpe ratio, efficient frontier, backtesting and ML were deliberately left out so the capstone fits in the time available.

## Tech

Python · NumPy · pandas · Plotly · Streamlit · yfinance · pytest · GitHub Codespaces · Streamlit Cloud

## Status

The working version is complete and its 36 tests pass. The dashboard preview in the Drive folder uses **synthetic data**. The live version with real NSE prices goes up once the app is deployed to Streamlit Cloud.

*Educational project. Not investment advice.*
