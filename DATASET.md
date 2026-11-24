# Dataset Documentation

## 2. Dataset Description

### Overview

This project uses historical cryptocurrency market data for three cryptocurrencies:

- Bitcoin (BTC)
- Ethereum (ETH)
- Solana (SOL)

The dataset is used to train and evaluate Machine Learning classification models.

### Dataset Features

The dataset contains the following columns:

| Feature | Description |
|---|---|
| Date | Date of the market observation |
| Coin | Cryptocurrency name |
| Close | Closing market price |
| Market_Cap | Cryptocurrency market capitalisation |
| Volume | Trading volume |
| Daily_Return | Daily percentage return |
| Indexed_Price | Normalised cryptocurrency price |
| MA_30 | 30-day moving average |
| MA_90 | 90-day moving average |
| Daily_Return_Decimal | Daily return in decimal form |
| Cumulative_Return | Cumulative market return |
| Running_Peak | Highest previous price |
| Drawdown | Decline from the running peak |

### Target Variable

The target variable is `Coin`.

It contains three classes:

- BTC
- ETH
- SOL

### Dataset Usage

The dataset will be used for:

1. Exploratory Data Analysis.
2. Feature selection.
3. Machine Learning classification.
4. Model evaluation and comparison.

### Important Note

The dataset is used to identify cryptocurrency classes, not to predict future cryptocurrency prices.
