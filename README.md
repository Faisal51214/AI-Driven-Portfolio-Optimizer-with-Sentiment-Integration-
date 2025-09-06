# AI Driven Portfolio Optimizer (with Sentiment Integration)

## Problem
Traditional portfolio optimization methods (such as mean–variance optimization) rely only on historical returns and covariances. They fail to account for the role of market psychology and sentiment, which often drive short-term volatility and major asset shifts.

## Method
I built an AI-driven portfolio optimizer that combines:
- Historical returns, volatility, and covariance (quantitative features)
- Sentiment analysis of financial news headlines (qualitative features)

Natural Language Processing (NLP) techniques were used to score sentiment (positive, neutral, negative). The optimizer integrates these sentiment-adjusted signals into a modern portfolio optimization algorithm.

## Results
- Portfolios achieved higher Sharpe ratios than baseline mean–variance optimizers.
- Sentiment integration reduced drawdowns during negative news cycles.
- Model demonstrated stability in allocation compared to sentiment-agnostic approaches.

## Future Work
- Use advanced NLP models such as FinBERT or GPT-based sentiment classifiers.
- Expand datasets to include social media feeds and analyst reports.
- Deploy the system as a web app with real-time optimization dashboards.
