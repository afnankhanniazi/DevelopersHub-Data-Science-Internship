# Bank Marketing Term Deposit Prediction

## Executive Summary
This project deploys a machine learning classification engine to predict whether retail banking customers will subscribe to a term deposit investment. By identifying the highest-probability targets and the underlying drivers of conversion, this analysis provides actionable strategies to optimize telemarketing resources and increase campaign ROI.

## Project Objective
To accurately predict customer subscription likelihood while identifying which specific demographic and engagement traits mathematically drive the final purchasing decision.

## Tech Stack & Architecture
- Language: Python 3
- Data Manipulation: pandas
- Feature Engineering: LabelEncoder, get_dummies (One-Hot Encoding)
- Machine Learning: scikit-learn (Random Forest Classifier)
- Data Visualization: matplotlib, seaborn

## Methodology
1. Data Preprocessing: Handled messy categorical text data by engineering binary and one-hot encoded numerical matrices suitable for machine learning ingestion.
2. Model Training: Deployed a Random Forest Classifier (n_estimators=100) using an 80/20 train-test split to prevent data leakage and overfitting.
3. Evaluation: Benchmarked the model using a comprehensive classification report, specifically optimizing for Recall on the positive ("Yes") class.
4. Insight Extraction: Mapped the feature_importances_ attribute to visually rank the top 10 biological/behavioral predictors.

## Performance Benchmarks

| Metric | Score | Business Context |
| :--- | :--- | :--- |
| Overall Accuracy | 84.10% | Highly robust baseline for behavioral data. |
| Recall ("Yes" Class) | 0.86 | Successfully identified 86% of all actual buyers. |
| Precision ("Yes" Class) | 0.81 | Strong confidence that predicted buyers are genuine. |

## Strategic Business Insights

- The Deciding Factors: The algorithm mathematically proved that Call Duration and Account Balance are the absolute dominant predictors of a subscription.
- Resource Optimization: The bank should immediately pivot from random dialing to highly targeted lists focusing on high-balance individuals. Additionally, telemarketing KPIs should shift to emphasize initial call engagement and duration, as keeping the customer on the line is the strongest predictive trigger for conversion.

---
This project was completed as part of the Advanced Data Science and Analytics track.
