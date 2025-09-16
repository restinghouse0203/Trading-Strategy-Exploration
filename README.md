# Trading-Strategy-Exploration

```markdown
# Quantitative Trading Strategies in Python & R

This repository explores and backtests various trading strategies and portfolio optimization techniques using Python and R.  
The goal is to build a research playground for quantitative finance, covering both single-asset trading strategies and multi-asset portfolio methods.

---

## Strategies Implemented

### Dummy Trade Strategy simulation experiment
- Binary Return Setup on basic trading strategy

### Technical Indicator-Based
- MACD Crossover (12, 26, 9)  
  - Buy when MACD line crosses above the signal line, sell when it crosses below.  
- RSI (Relative Strength Index)  
  - Buy when RSI < 30 (oversold), sell when RSI > 70 (overbought).  

### Statistical Arbitrage
- Pair Trading (Cointegration-based)  
  - Identify cointegrated stock pairs and trade the spread.  

### Portfolio Optimization
- Markowitz Mean-Variance Optimization  
  - Efficient frontier construction, portfolio risk-return tradeoff, and comparison with equal-weighted portfolios.  

---

## Tech Stack
- Python 3.11
- [Backtrader](https://www.backtrader.com/) – backtesting engine  
- [yfinance](https://github.com/ranaroussi/yfinance) – historical stock data  
- `pandas`, `numpy`, `scipy` – data analysis & statistics  
- `matplotlib`, `seaborn`, `plotly` – visualization  
- `cvxpy` / `PyPortfolioOpt` – portfolio optimization  

---

## Project Structure


quant-strategies/
│── data/                   # Stored market data (optional)
│── notebooks/              # Jupyter notebooks with backtests & analysis
│   ├── macd\_strategy.ipynb
│   ├── rsi\_strategy.ipynb
│   ├── pair\_trading.ipynb
│   ├── markowitz\_portfolio.ipynb
│── src/                    # Python modules for strategies & utils
│── README.md               # Project documentation (this file)
│── requirements.txt        # Python dependencies



---

## Performance Evaluation
Each strategy is evaluated with:
- PnL (Profit & Loss)  
- Sharpe Ratio  
- Max Drawdown  
- Win Rate  
- Equity Curve Visualization**  

For portfolio strategies:
- Efficient Frontier plots  
- Risk-return scatter  
- Asset allocation weights  
---

## Notes
- Backtrader provides realistic **broker simulation**, so results differ from simple vectorized backtests.  
- Vectorized pandas backtests are also included for comparison and faster prototyping.  

---

##� Roadmap
- Add Bollinger Bands strategy  
- Implement Kalman filter-based pair trading  
- Compare strategies vs. **buy-and-hold benchmark  
- Add live-paper trading integration (e.g., with Alpaca API)  

---

## License
MIT License – free to use and modify.  
```
