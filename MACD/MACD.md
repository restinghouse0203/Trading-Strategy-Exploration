# Algorithmic Trading Project – MACD Strategy on IBM

This project implements and backtests a simple **MACD (12, 26, 9) crossover trading strategy** on **IBM stock data** using Python and the **Backtrader** framework.  

The goal is to demonstrate a full trading research pipeline:
1. Data acquisition  
2. Strategy implementation  
3. Backtesting with a broker simulator  
4. Performance evaluation (PnL, Sharpe ratio, Drawdown, Win rate, etc.)  
5. Visualization of trading signals, MACD, and portfolio equity  

---

## 📈 Strategy Description
The MACD indicator is defined as:

- **MACD Line** = 12-day EMA – 26-day EMA  
- **Signal Line** = 9-day EMA of MACD Line  

Trading rules:
- **Buy** when the MACD line crosses **above** the Signal line  
- **Sell** when the MACD line crosses **below** the Signal line  

---

## ⚙️ Tech Stack
- **Python 3.11+**  
- [Backtrader](https://www.backtrader.com/) – Backtesting framework  
- [yfinance](https://github.com/ranaroussi/yfinance) – Historical stock data  
- `matplotlib`, `pandas` – Visualization and data analysis  

---

📊 Performance Evaluation
The strategy produces the following key metrics:

- Final Portfolio Value

- PnL (Profit & Loss)

- Sharpe Ratio

- Maximum Drawdown (absolute and %)

- Win rate of trades

- Average profit/loss per trade

Results are summarized in a performance table and visualized with:

- Equity curve over time

- Drawdown chart

- MACD + Signal line overlayed on price


