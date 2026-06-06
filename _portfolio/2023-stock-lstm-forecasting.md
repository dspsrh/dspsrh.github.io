---
title: "Stock-Price Forecasting with Stacked LSTMs"
excerpt: "Four-layer stacked LSTM for next-step price forecasting on GOOG and ORCL."
collection: portfolio
---

**[View code on GitHub](https://github.com/dspsrh/stock_prediction_model)**

Personal project · TensorFlow / Keras

* Built a stacked four-layer LSTM (50→60→80→120 units) with dropout regularization to forecast next-step prices for Google (GOOG) and Oracle (ORCL) from multivariate OHLCV inputs.
* Engineered the sequence-windowing and normalization pipeline and trained per-ticker models under a mean-squared-error objective.
