# AI Driven Portfolio Optimizer (with Sentiment Integration)

## Problem
Traditional portfolio optimization methods (such as mean–variance optimization) rely only on historical returns and covariances. They fail to account for the role of market psychology and sentiment, which often drive short-term volatility and major asset shifts.
This project explores sentiment-aware portfolio optimization for four major technology companies:
- Apple (AAPL)  
- Microsoft (MSFT)  
- Alphabet (GOOGL)  
- Amazon (AMZN)  

## Data
- **Price data**: Daily OHLCV (3 years) from Yahoo Finance via `yfinance`.  
- **News data**: scraped / sample financial headlines related to AAPL, MSFT, GOOGL, AMZN
- **Sentiment analysis**: VADER sentiment analysis

## Method
- yfinance (Adjusted Close → returns)
- PyPortfolioOpt (mean-variance optimization)
- VADER sentiment from sample headlines (CSV)
- Weight adjustment logic (prototype, not fully tested)

## Results
- **Annualized stock returns**:  
  - AAPL: 13.95%  
  - MSFT: 23.57%  
  - GOOGL: 23.08%  
  - AMZN: 22.17%  

- **Max Sharpe portfolio (baseline)**:  
  - Expected Return: **23.42%**  
  - Volatility: **25.10%**  
  - Sharpe Ratio: **0.85**

The notebook demonstrates feasibility of sentiment-adjusted allocation but does not fully backtest the sentiment overlay.  

## Future Work
- Walk-forward backtests with rolling sentiment adjustment.  
- FinBERT transformer for richer sentiment signals.  
- Include transaction costs and rebalance schedules.  
- Extend to a larger universe of assets.  

