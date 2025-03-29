# TechnicalAnalysisTradingProject

**SentimentPicker** is a stock trading signal generator that uses technical indicators and backtesting to evaluate a simple strategy. It focuses on sentiment derived from technical signals rather than social media or news sentiment.

## Features
- Downloads historical stock data using `yfinance`
- Computes technical indicators like:
  - RSI (Relative Strength Index)
  - SMA20 and SMA50 (Simple Moving Averages)
  - Bollinger Bands (Upper, Middle, Lower)
- Applies a custom strategy using `Backtrader`:
  - Buys when RSI < 30 and price is near the lower Bollinger Band
  - Sells when RSI > 70 and price is near the upper Bollinger Band
- Visualizes strategy performance and overlays buy/sell signals

- `pandas`, `numpy`, `matplotlib`, `yfinance`  
- `TA-Lib` (technical analysis library)  
- `backtrader`
- `newsapi`
- `huggingface`

## Usage
1. Open the Jupyter notebook `SentimentPicker.ipynb`
2. Modify the `ticker`, `start_date`, and `end_date` to suit your analysis
3. Run all cells to compute indicators, apply the strategy, and view backtest results

## Notes
This project defines "sentiment" based on recent news sentiment about a stock
