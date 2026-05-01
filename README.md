# Oil Price Trend Scanner
A quantitative scanner that detects trend reversals in Brent Crude Oil (BZ=F) using a moving average crossover strategy.
How it works

## How it works
Downloads 1 year of daily OHLCV data via yfinance
Computes a 40-day and 90-day rolling average on the closing price
Generates a binary signal: +1 (bullish) when MA40 > MA90, -1 (bearish) otherwise
Detects crossover events (signal diff = ±2) that flag a potential trend reversal
