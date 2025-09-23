# Portfolio Risk Metrics

This project analyzes a simple 3-stock portfolio (Apple, Microsoft, Amazon) to demonstrate fundamental risk and return concepts used in quantitative finance. Portfolio analysis is not only about how much return was acheived, but also about how much risk was taken to get that return. By adding VaR and CVaR, this project goes beyond basic metrics and demonstrate understanding of **tail risk**, which is critical in professional risk management and quantitative finance.


## Phase 1: Basic Portfolio Metrics
- Built a portfolio with weights: AAPL (40%), MSFT (30%), AMZN (30%)
- Calculated **daily returns** from stock price data
- Computed **portfolio returns** using weighted averages
- Analyzed **cumulative portfolio growth** starting with a $1 investment
- Measured **risk-adjusted performance** using:
  - Annualized Return: 0.3146
  - Annualized Volatility: 0.1894
  - Sharpe Ratio: 1.3968


## Phase 2: Value at Risk (VaR) and Conditional VaR (CVaR)
- Implemented **Historical VaR** (95%, 99%)
- Implemented **Parametric VaR** (95%, 99%) using normal distribution assumption
- Calculated **Conditional VaR (CVaR, Expected Shortfall)**
- Visualized the return distribution with VaR and CVaR cutoff lines

**Key Insights**
- Historical VaR (95%): -2% → 5% chance daily loss exceeds –2%
- Historical VaR (99%): –3.4% → 1% chance daily loss exceeds –3.4%
- CVaR (95%): –2.9% → average loss if the 5% worst days occur
- CVaR (99%): –3.8% → average loss if the 1% worst days occur


## Tools
Python (pandas, yfinance, matplotlib, numpy)
