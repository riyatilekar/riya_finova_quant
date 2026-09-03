# FINOVA Quant & Trading Committee — Domain Task
## The Chart Detective: 20/50 EMA Crossover Backtest

## Repository structure
reliance_trade_log.xlsx   - Trade log + 5 summary stats
code/                     - Python script / notebook used to generate the results
screenshots/               - Full 12-month chart, best trade, worst trade
README.md                 - This file (approach, results, verdict)

## Approach
Used a Python script (yfinance + pandas) instead of manually reading the TradingView chart, to avoid missing or misjudging crossovers by eye. Pulled 24 months of RELIANCE daily data and trimmed to the real last 12 months so the EMAs are fully warmed up before counting trades.

## Results
- Instrument: RELIANCE
- Total trades: 2
- Number of winners: 0
- Win rate: 0%
- Best trade (least bad): -0.44% (Oct 21, 2025 to Jan 15, 2026)
- Worst trade: -5.5% (May 6, 2026 to May 13, 2026)

Both trades lost money. See reliance_trade_log.xlsx for the full trade log and summary
stats.

## Verdict
RELIANCE | 2 Trades | 0% Win Rate | [your one-line verdict here]

[Your verdict paragraph goes here, in your own words.]
