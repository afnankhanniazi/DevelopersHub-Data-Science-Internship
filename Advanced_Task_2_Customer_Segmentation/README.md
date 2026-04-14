# ⚡ Energy Consumption Time Series Forecasting

## 📌 Executive Summary
This project engineers a machine learning pipeline to forecast short-term household energy consumption. By comparing classical statistical models against modern machine learning and advanced forecasting algorithms, this analysis determines the most efficient approach for predicting utility grid demands based on human behavioral patterns.

## 🎯 Business Objective
To optimize power distribution and minimize grid overload by accurately predicting daily energy usage spikes (e.g., winter heating, weekend activity) using historical time-series data.

## 🛠️ Tech Stack & Architecture
- **Language:** Python 3
- **Data Manipulation:** `pandas`, `numpy`
- **Machine Learning:** `xgboost`, `scikit-learn`
- **Advanced Forecasting:** `prophet` (Meta)
- **Classical Statistics:** `statsmodels` (ARIMA)
- **Data Visualization:** `matplotlib`

## 🗄️ Dataset Details
- **Source:** Household Power Consumption Dataset
- **Frequency:** Resampled to daily aggregates to reduce noise and isolate macro-trends.
- **Preprocessing Applied:** Forward-fill imputation for missing intervals to ensure chronological integrity.
- **Engineered Features:** Extracted `month`, `day_of_week`, and constructed a binary `is_weekend` indicator to capture behavioral spikes.

## ⚙️ Methodology
1. **Exploratory Data Analysis (EDA):** Identified heavy overlapping seasonalities (yearly climate trends + weekly human routines).
2. **Feature Engineering:** Translated chronological index data into actionable machine learning features.
3. **Model Training:** Deployed three distinct forecasting architectures on a 75/25 chronological train-test split.
4. **Evaluation:** Benchmarked predictive accuracy using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## 📊 Performance Benchmarks

| Model Architecture | MAE (Kilowatts) | RMSE (Kilowatts) | Performance Tier |
| :--- | :--- | :--- | :--- |
| **Meta's Prophet** | **86.79** | **107.69** | 🏆 **Optimal** |
| **XGBoost** | 92.00 | 114.14 | Highly Accurate |
| **ARIMA (7,1,0)** | 176.81 | 215.23 | Baseline/Insufficient |

## 💡 Strategic Business Insights

- **The Winner:** **Meta's Prophet** is the recommended model for deployment. It successfully captured both the weekly human usage patterns and the broader seasonal waves with the lowest error rate.
- **The Machine Learning Advantage:** Both Prophet and XGBoost drastically outperformed the classical ARIMA model. 
- **The "Why":** ARIMA struggles with overlapping seasonalities (e.g., weekend spikes occurring simultaneously with winter surges). Modern machine learning tools are strictly required for accurate, real-world utility forecasting.

---
*This project was completed as part of the Advanced Data Science and Analytics track.*
