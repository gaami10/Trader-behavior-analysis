# Trader Behavior Insights — Draft Report

**Candidate:** Aditya (Gaami) Sawant  
**Dataset:** Hyperliquid historical trades + Bitcoin Fear & Greed Index

## Objective
Analyze how trader behavior (profitability, risk, volume, leverage) aligns with market sentiment (Fear vs Greed).

## Key preliminary findings (from EDA)
- Greed days (value ≥60) show **higher average profit** and slightly **higher probability of profitable trades** compared to Fear days in this dataset.
- Example aggregated numbers (approx):
  - Fear: avg profit ≈ 50 USD, win rate ≈ 41.5%
  - Neutral: avg profit ≈ 22 USD, win rate ≈ 31.7%
  - Greed: avg profit ≈ 77.8 USD, win rate ≈ 45.4%
- Buy ratio is slightly **higher in Fear** and lower in Greed (shorting/less buys in Greed).

## Next steps performed in notebook_1.ipynb
1. Data loading, parsing timestamps (Unix ms), merging daily sentiment.
2. Feature engineering: return_pct, notional_usd, lagged sentiment (1–3 days), rolling sentiment (7/14 days).
3. EDA and statistical tests (ANOVA / Kruskal-Wallis recommended).
4. Predictive modeling (Logistic Regression / Random Forest) to predict profitable trades.
5. Actionable recommendations based on results.

## Recommendations (short)
- Use sentiment as a risk overlay: reduce leverage on extreme Greed days.
- Monitor 3-day sentiment drops as short-term reversal signals.
- Further work: incorporate BTC price volatility, order-level holding times, and trader clustering.

(Full details, code, and charts available in notebook_1.ipynb)
