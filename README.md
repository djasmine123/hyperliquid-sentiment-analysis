# Hyperliquid Trader Performance vs Fear & Greed Index Analysis

## Overview

This project analyzes the relationship between cryptocurrency market sentiment and trader performance using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.

The objective is to determine whether different market sentiment regimes (Fear, Greed, etc.) influence trading profitability and behavior, and to identify patterns that can support better trading decisions.

---

## Objective

- Merge historical Hyperliquid trading data with the Bitcoin Fear & Greed Index.
- Evaluate trader performance across different market sentiment regimes.
- Identify hidden trading patterns.
- Generate actionable insights for trading strategy.

---

## Datasets

### 1. Historical Hyperliquid Trading Data

Contains:

- Account
- Symbol
- Execution Price
- Size
- Side
- Timestamp
- Start Position
- Closed PnL
- Leverage
- Direction
- Event

### 2. Bitcoin Fear & Greed Index

Contains:

- Date
- Market Sentiment Classification
  - Extreme Fear
  - Fear
  - Neutral
  - Greed
  - Extreme Greed

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab

---

## Project Workflow

### 1. Data Loading
- Import both datasets
- Parse date columns
- Inspect missing values

### 2. Data Preparation
- Standardize date formats
- Merge sentiment data with historical trades
- Remove unmatched records

### 3. Performance Analysis
- Filter closing trades
- Calculate:
  - Win Rate
  - Average Profit (PnL)
  - Total Profit
  - Number of Trades

### 4. Market Sentiment Analysis
Evaluate trader performance across:

- Extreme Fear
- Fear
- Neutral
- Greed
- Extreme Greed

### 5. Trading Bias Analysis
Analyze:

- Open Long Positions
- Open Short Positions
- Long Position Percentage

### 6. Account-Level Analysis
Identify:

- Sentiment-sensitive traders
- Stable (sentiment-agnostic) traders
- Overall profitable accounts

### 7. Visualization
Generate bar charts showing:

- Win Rate by Sentiment
- Average PnL by Sentiment
- Long Position Percentage by Sentiment

---

## Key Findings

- **Fear** recorded the highest trading performance with:
  - Highest win rate
  - Highest average profit per trade

- **Greed** produced the weakest trading performance.

- Traders opened more long positions during Fear (76.2%) than during Greed (70.6%), suggesting a contrarian trading behavior.

- 20 out of 22 trader accounts were profitable overall.

- Some accounts maintained relatively stable performance across sentiment regimes, while others showed significant sensitivity to market sentiment.

---

## Business Insight

Market sentiment does influence trading performance, but not uniformly across all traders.

The analysis suggests:

- Increasing position size during Fear periods may improve returns.
- Reducing exposure during Greed periods may help manage risk.
- Monitoring account-level sensitivity to sentiment can support more adaptive trading strategies.

---

## Repository Structure

```
Hyperliquid-Trader-Sentiment-Analysis/
│
├── Hyperliquid_Trader_Sentiment_Analysis.ipynb
├── README.md
└── requirements.txt
```

---

## Results

The notebook provides:

- Data preprocessing
- Feature engineering
- Exploratory data analysis
- Sentiment-based performance metrics
- Account-level consistency analysis
- Visualizations
- Business recommendations

---

## Author

**Jasmine D**

Data Science Graduate
