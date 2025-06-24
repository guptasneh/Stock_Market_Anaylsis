#  Trader Behavior 

##  Project Summary

This project investigates how Bitcoin market sentiment (Fear vs. Greed) affects trading behavior and performance. We integrate two datasets:

- **Fear-Greed Index**: Tracks daily sentiment classification (Fear or Greed).
- **Hyperliquid Trader Data**: Provides detailed records of trades (e.g., execution price, size, leverage, PnL, etc.)

The goal is to uncover patterns between emotional market states and risk-taking decisions to help build smarter, sentiment-aware trading strategies in the Web3 ecosystem.


##  Dataset Overview

### 1. Fear-Greed Index
- **Columns**: `Date`, `Classification`
- Represents the overall emotional tone of the crypto market per day.

### 2. Hyperliquid Historical Trader Data
- **Columns** include:
  - `account`, `symbol`, `execution price`, `size`, `side`, `time`
  - `start position`, `event`, `closedPnL`, `leverage`, etc.
- Allows us to assess individual trader behavior and profitability.

---

##  Key Findings from the Analysis

   Sentiment Affects Trading Behavior:
- On Greed Days:
  - Traders tend to 'increase leverage' and 'trade larger positions'.
  - 'More trades' are executed overall, reflecting higher market participation.
  - Average 'PnL per trade' is higher, but so is volatility.

- On **Fear Days**:
  - Traders shift to 'short positions' and trade less frequently.
  - Some 'contrarian traders' perform better, capitalizing on emotional overreactions.

###  Leverage & Risk Appetite:
- Higher leverage usage is prominent during **Greed**, showing optimism.
- During **Fear**, most traders reduce exposure or avoid risky setups.

###  Behavioral Clustering:
Using K-Means, traders were grouped into:
1. **Aggressive**: High leverage, high volume, variable profits.
2. **Cautious**: Low-risk trades, smaller sizes, steady gains/losses.
3. **Opportunists**: Fewer trades, but timed well with sentiment shifts.

###  Time-Based Patterns:
- Trading activity increases during **rallies on Greed days**.
- Fear-based trading is more spread out, likely reactionary.


##  Tools & Libraries Used

-  Python
-  Pandas, NumPy – data preprocessing
-  Matplotlib, Seaborn, Plotly – data visualization
-  Scikit-learn – clustering & basic modeling


##  Strategic Takeaways

- Market sentiment is a **strong predictor of trader behavior and performance**.
- **Leverage and trade size** can be monitored as risk signals.
- A small set of **traders consistently profit in Fear markets**, offering potential modeling value.
- Integrating sentiment into platforms could help build **personalized trading alerts** and **strategy filters**.



