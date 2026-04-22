# Trade-Sentiment
Data analysis of Bitcoin Fear &amp; Greed sentiment vs Hyperliquid trader behavior. Includes PnL analysis, trader segmentation, and strategy insights.
# Trader Behavior vs Market Sentiment Analysis

## Objective

This project analyzes the relationship between Bitcoin market sentiment (Fear vs Greed) and trader behavior on Hyperliquid.

The goal is to identify patterns in trader performance and behavior that could inform smarter trading strategies.

---

# Dataset

Two datasets were used:

### 1. Bitcoin Fear & Greed Index

Contains daily sentiment classification of the crypto market.

Columns:

* Date
* Classification (Fear / Greed)

### 2. Hyperliquid Trader Data

Historical trade data including:

* Account
* Coin
* Execution Price
* Trade Size
* Side (Buy/Sell)
* Closed PnL
* Timestamp

---

# Methodology

### Data Cleaning

* Standardized column names
* Converted timestamps to datetime
* Extracted daily dates for merging
* Removed rows with missing sentiment

### Dataset Alignment

Both datasets were aligned on **daily timestamps** to merge trader behavior with market sentiment.

### Feature Engineering

Key metrics were created:

* Daily PnL per trader
* Win rate
* Trade frequency
* Average trade size
* Long vs short ratio

### Trader Segmentation

Traders were grouped into segments:

* High vs low trade size
* High-frequency vs low-frequency traders
* Winning vs losing traders

---

# Key Insights

### Insight 1: Higher trading activity during Greed

Trade frequency increases significantly during Greed periods, suggesting traders become more active in bullish sentiment.

### Insight 2: Larger PnL volatility during Fear

PnL distribution shows higher variance during Fear days, indicating higher market instability.

### Insight 3: High-frequency traders perform more consistently

Frequent traders demonstrate more stable performance compared to infrequent traders.

---

# Strategy Recommendations

### Strategy 1: Reduce position sizes during Fear

Fear periods exhibit higher volatility and loss potential. Reducing trade size may improve risk-adjusted returns.

### Strategy 2: Avoid overtrading during Greed

Greed periods encourage excessive trading. Limiting trade frequency may help avoid sentiment-driven decisions.

---

# How to Run

Install dependencies:

pip install -r requirements.txt

Run the notebook:

Open notebook/analysis.ipynb

---

# Output

The notebook generates charts including:

* PnL distribution by sentiment
* Trade frequency by sentiment
* Long vs short trading bias

These visualizations highlight behavioral differences between Fear and Greed market conditions.
