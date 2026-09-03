# FINOVA Quant & Trading Committee: Domain Task

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

This strategy is good for catching that the prices are rising however it cannot predict whether they would continue rising or not. In the case of reliance and many other companies in nifty 50 such as tatamotors, infosys etc. this strategy fails more often than it succeeds. I think it catches on to the rising prices too late. By the time it realises the prices have already started falling.

This kind of strategy would be good for a market where the prices are stable and continue their trends without drastic changes.

It's strength is that it catches the rising prices really well. It's weakness is that it cannot predict whether they will continue rising or not. Also it takes a while for it to realise they are falling. Also another weakness is that we trade whenever it crosses, regardless of how strong or weak that move actually is, there is no filter for how convincing the signal is. It also has no risk management built in, once you're in a trade it just holds until the next crossover no matter how far the price moves against you, there's no stop loss to cut a losing trade early.

I would not trade this strategy with my own money.

