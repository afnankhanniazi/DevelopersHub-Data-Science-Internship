# DevelopersHub Data Science & Analytics Portfolio

## 📌 Overview
This repository contains my completed portfolio projects for the Data Science & Analytics Program at DevelopersHub Corporation. The tasks demonstrate end-to-end data pipeline competencies: from raw data ingestion and exploratory data analysis (EDA), to advanced machine learning modeling, time-series forecasting, and interactive deployment.

## 👨‍💻 About Me
As a final-year Computer Science student actively pursuing Graduate Trainee and Junior Data Scientist roles, my objective is to bridge the gap between complex mathematical algorithms and actionable business intelligence. 

## 🛠️ Technical Arsenal
- **Languages:** Python
- **Data Engineering:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn` (Logistic/Linear Regression, Random Forest, K-Means)
- **Advanced Forecasting:** `xgboost`, `prophet` (Meta), `statsmodels` (ARIMA)
- **Evaluation:** Confusion Matrices, Accuracy Scoring, RMSE/MAE, Feature Importance Extraction
- **Deployment:** IPyWidgets (Interactive Colab GUIs)

---

## 🚀 Phase 2: Advanced Tasks

### 1. Term Deposit Subscription Prediction (Bank Marketing)
- **Objective:** Predict whether retail banking customers will subscribe to a term deposit investment to optimize telemarketing resources.
- **Algorithm:** Random Forest Classifier.
- **Key Insight:** Achieved 84.10% overall accuracy and successfully identified 86% of actual buyers. Proved mathematically that Call Duration and Account Balance are the dominant predictors of conversion, signaling a critical need to pivot to targeted, high-balance calling lists.

### 2. Customer Segmentation (Unsupervised Learning)
- **Objective:** Group mall customers based on spending habits to optimize marketing ad spend.
- **Algorithm:** K-Means Clustering (Optimized via the Elbow Method).
- **Key Insight:** Successfully mathematically segmented the customer base into 5 distinct buyer profiles (e.g., VIPs, Frugal, Impulse Buyers), directly translating abstract clusters into highly targeted marketing strategies.

### 3. Energy Consumption Forecasting (Time-Series)
- **Objective:** Predict short-term utility grid demands based on historical household usage.
- **Algorithms Tested:** Meta's Prophet, XGBoost, and ARIMA.
- **Key Insight:** Meta's Prophet outperformed XGBoost and traditional ARIMA by successfully capturing overlapping weekly human routines (weekend spikes) and yearly climate seasonality, proving classical statistics are insufficient for modern grid forecasting.

---

## 🏗️ Phase 1: Foundation Tasks

### 1. Iris Species Classification (Supervised Learning)
- **Objective:** Classify botanical species based on physical dimensions.
- **Algorithm:** Random Forest Classifier.
- **Key Insight:** Achieved 100% predictive accuracy. Extracted internal feature importance to prove that petal dimensions are the sole biological indicators required, allowing future researchers to abandon sepal measurements and optimize data collection.

### 2. Credit Risk and Loan Approval Prediction
- **Objective:** Engineer a classification engine to predict bank loan defaults and minimize institutional risk.
- **Algorithm:** Logistic Regression (82.83% Baseline Accuracy).
- **Key Insight:** Extracted model coefficients to prove historical credit behavior vastly outweighs raw income. Engineered a **Live Interactive Prediction Engine GUI** to allow end-users to input financial parameters and receive real-time approval inferences.

### 3. Medical Insurance Cost Prediction
- **Objective:** Estimate medical insurance claim amounts based on demographic profiles.
- **Algorithm:** Linear Regression.
- **Key Insight:** Isolated "Smoking Status" as a massive, overriding cost multiplier, proving that actuarial premium pricing models must strictly segment smokers into distinct, high-cost risk pools to maintain profitability.

---
*Thank you for reviewing my portfolio. Please explore the individual project directories for detailed Jupyter Notebooks, fully commented Python code, and interactive visual deployments.*
