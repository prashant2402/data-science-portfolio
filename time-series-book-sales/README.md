# 📚 Time Series Forecasting – Book Sales Analysis (Nielsen Dataset)

This project explores advanced time series forecasting techniques on weekly sales data for 500 books across four major categories using Nielsen BookScan-style data. It was developed as part of the **University of Cambridge Data Science Career Accelerator**.

Two standout titles — *The Alchemist* and *The Very Hungry Caterpillar* — are examined in depth to identify seasonal trends and build predictive models to guide **inventory planning and demand forecasting** for small to mid-sized publishers.

---

## 🔍 Project Highlights

- Forecasted 32 weeks of weekly book sales using:
  - ✅ **SARIMA / ARIMA**
  - ✅ **XGBoost**
  - ✅ **LSTM Neural Networks**
  - ✅ **Hybrid Parallel + Sequential Models (SARIMA + LSTM)**
- Decomposed series into **trend, seasonality, and noise**
- Compared **weekly vs monthly** forecasting granularity
- Applied ACF/PACF and stationarity tests
- Evaluated performance using **MAPE, RMSE, visual alignment**

---

## 📈 Key Results

| Title                  | Model         | MAPE (%) |
|------------------------|---------------|----------|
| The Alchemist          | XGBoost       | 1.59     |
| The Very Hungry Caterpillar | XGBoost   | 1.89     |
| The Alchemist          | SARIMAX       | 27.15    |
| Caterpillar            | SARIMAX       | 16.60    |
| Both Titles            | LSTM          | ~19.00   |

> 📌 Parallel hybrids performed best when mixing SARIMA + LSTM.
> 📦 Granular weekly models outperformed monthly predictions across the board.

---

## 🛠️ Tools & Techniques

- Time Series Decomposition
- SARIMA / SARIMAX (statsmodels)
- XGBoost Regression
- LSTM Forecasting (TensorFlow / Keras)
- Hybrid model blending
- Lag features, cyclical encodings, trend windows

---

## 📎 Acknowledgments

This project was completed during the **University of Cambridge x FourthRev** Data Science Career Accelerator (2024 cohort).
