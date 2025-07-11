## 🏬 Store Sales Time Series Forecasting
Forecasting daily item sales across multiple stores using advanced machine learning and time-series analysis.

---

## 📌 Overview
This project builds an end-to-end sales forecasting system using real-world data from the Favorita Grocery Sales Forecasting challenge.

It is designed to simulate a real Amazon-style data science workflow, emphasizing modeling, forecasting accuracy, business insight, and explainability.


---

## 🎯 Objective
Predict the daily sales of products across stores, leveraging:

Past sales trends

Promotions

Transactions

Oil prices

Calendar-based features (day, month) 

---

# 🧠 Features

| Component                   | Description                                                  |
|---------------------------  |--------------------------------------------------------------|
| 📈 Forecasting Model       | Gradient Boosted Trees via **XGBoost**                       |
| 🔂 Cross-validation        | `TimeSeriesSplit` to mimic future forecasting                |
| 🧹 Feature Engineering     | Lag variables, rolling averages, calendar data               |
| 📊 Evaluation              | MAE, RMSE, R² + visual plots                                 |
| 🔁 Naive Baseline          | Lag-1 based naive forecast for model comparison              |
| 📉 Error Analysis          | MAE breakdown by `store_nbr` and `family`                    |
| 🗃️ SQL Integration         | DuckDB + Pandas for fast analytics                           |
| 🖼️ Actual vs Predicted     | Visual comparison of predicted vs true sales                 |

---

## 🧰 Tech Stack

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- XGBoost
- scikit-learn
- DuckDB (for SQL analysis)
- Streamlit (optional future deployment)
- Google Colab (development)

---

## 🧪 Model Performance

| Model           | MAE     | RMSE    | R²    |
|-----------------|---------|---------|-------|
| Naive Forecast  | 1210.57 | 1789.46 | 0.79  |
| XGBoost (CV)    | 1034.34 | 1612.88 | 0.85  |

✅ **~14.6% reduction in RMSE** over the naive baseline

---


## 🧠 Business Insight

> “Product families like `BEVERAGES` and stores in region `Quito` showed higher forecasting error — indicating volatility or promotion-driven spikes.”

---

## 🚀 Future Work

- 🔍 Add SHAP explainability for feature-level insights
- 🗺️ Regional forecasting decomposition
- ⏱️ Hyperparameter optimization with Optuna
- 🧠 Try LSTM/Transformer-based sequence models

---

## 📄 Resume-Ready Bullet

> ✅ Built an end-to-end sales forecasting pipeline using XGBoost and TimeSeriesSplit CV, improving RMSE by 14.6% over a naive baseline. Performed business-level error analysis and actual vs predicted trend visualization to diagnose model weaknesses across stores and product lines.

---

## 📎 Links

- 📊 [Kaggle Dataset](https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data)
- 🔗 [Project Notebook (Colab)](https://colab.research.google.com/drive/17mVbD2-iPr3c8Af2SsDfdAh8cL0tHG5U?usp=sharing)

---

## 🙌 Credits

Inspired by Amazon-style demand forecasting problems and data-driven decision science practices.



