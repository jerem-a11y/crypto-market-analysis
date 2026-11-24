# Cryptocurrency Classification

## Project Overview

This project explores the use of machine learning to classify three cryptocurrencies: Bitcoin (BTC), Ethereum (ETH), and Solana (SOL), using historical market data.

The goal is to train and compare different classification models and evaluate how accurately they can identify each cryptocurrency from its market features.

## Dataset

- **Cryptocurrencies:** BTC, ETH, SOL
- **Date range:** January 1, 2021 – December 31, 2025
- **Total records:** 5,478
- **Records per cryptocurrency:** 1,826

## Features

The dataset includes:

- Close
- Market_Cap
- Volume
- Daily_Return
- Indexed_Price
- MA_30
- MA_90
- Daily_Return_Decimal
- Cumulative_Return
- Running_Peak
- Drawdown

## Data Splitting

The dataset was split chronologically to keep the test period after the training period.

- **Training records:** 4,380
- **Testing records:** 1,098
- **Training period:** January 1, 2021 – December 30, 2024
- **Testing period:** December 31, 2024 – December 31, 2025

## Models Trained

Four classification algorithms were evaluated:

1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine (SVM)

## Model Results

| Model | Accuracy |
|---|---:|
| Logistic Regression | 100% |
| Decision Tree | 100% |
| Random Forest | 100% |
| SVM | 100% |

These are the reported results using the full feature set.

A separate Random Forest experiment using only Close, Market_Cap, and Volume achieved **99.73% accuracy**.

## Random Forest Feature Importance

The most influential features in the Random Forest experiment were:

1. Market_Cap
2. Close
3. MA_30
4. Running_Peak
5. MA_90

## Confusion Matrix

The Random Forest confusion matrix for the test set was:

```text
[[366,   0,   0],
 [  0, 366,   0],
 [  0,   3, 363]]
```

The model correctly classified 1,095 out of 1,098 test records.

## Conclusion

This project demonstrates how machine learning classification algorithms can use cryptocurrency market data to distinguish between BTC, ETH, and SOL.

The four models achieved 100% reported accuracy using the full feature set, while a simpler Random Forest model achieved 99.73% accuracy using only three features.

**Important:** This is a cryptocurrency classification project. It does not predict future cryptocurrency prices or guarantee trading performance.

The results should be interpreted carefully, and the data-splitting and preprocessing pipeline should be checked for possible data leakage before treating the reported accuracy as a reliable measure of generalization.
