# DevelopersHub Data Science & Analytics Internship

## Overview
This repository contains my completed portfolio projects for the Data Science & Analytics Internship at DevelopersHub Corporation. 

The tasks within this repository are designed to demonstrate core competencies in the data science pipeline. This includes data loading, exploratory data analysis (EDA), data cleaning, feature encoding, machine learning model training, and performance evaluation. 

## About Me

Welcome to my data science portfolio! As a final-year Computer Science student actively pursuing Graduate Trainee and Junior Officer opportunities in the tech industry, I built this repository to document my completed projects for the Data Science and Analytics Internship at DevelopersHub Corporation. 

The tasks within this repository are structured to demonstrate a comprehensive understanding of the end-to-end data pipeline: from raw data ingestion and missing value imputation, to advanced feature engineering, predictive modeling, and interactive deployment. My goal is to bridge the gap between complex mathematical algorithms and actionable business intelligence.

## Technical Arsenal

- Languages: Python
- Data Engineering and Manipulation: pandas, numpy
- Data Visualization and EDA: matplotlib, seaborn
- Machine Learning Algorithms: scikit-learn (Logistic Regression, Linear Regression)
- Model Evaluation: Confusion Matrices, Accuracy Scoring, RMSE, MAE, Feature Coefficient Extraction
- Deployment and Interactive UI: IPyWidgets (Colab Forms)

## Detailed Project Breakdown

### Task 1: Advanced EDA on the Iris Dataset

- Objective: Perform rigorous Exploratory Data Analysis (EDA) to mathematically and visually identify distinctions between biological species.
- Technical Approach: Loaded structured data, verified integrity, and deployed standard distribution visualizations (scatter plots, histograms, box plots). Escalated the analysis by implementing multidimensional clustering techniques using Seaborn Pairplots and generating a Feature Correlation Heatmap.
- Deep Business and Technical Insight:
  - Feature Redundancy: The correlation heatmap mathematically proved a nearly perfect positive correlation (0.96) between petal length and petal width. 
  - Strategic Impact: In a real-world scenario with massive biological datasets, this insight allows us to safely drop one of these features to reduce computational load (dimensionality reduction) without sacrificing the predictive power of future classification models. It proves that petal dimensions are the ultimate isolating indicators for this dataset.

### Task 2: Credit Risk and Loan Approval Prediction

- Objective: Engineer a machine learning classification engine to predict bank loan defaults, minimizing institutional financial risk.
- Technical Approach: Addressed messy real-world data by imputing missing continuous variables with medians and categorical variables with modes. Applied One-Hot Encoding to prepare the data matrix. Trained a Logistic Regression classifier, achieving a highly robust baseline accuracy of 82.83%. 
- Standout Feature (Live UI): Engineered a Live Interactive Prediction Engine directly within the notebook. This GUI allows end-users to input custom financial parameters via sliders and receive real-time loan approval inferences and statistical confidence scores.
- Deep Business and Technical Insight: 
  - The Black Box Opened: By extracting the model's mathematical coefficients, the data revealed that Credit History vastly outweighs raw Applicant Income or Loan Amount. 
  - Strategic Impact: This indicates that historical financial behavior is a far superior predictor of future reliability than current financial capability. From a banking risk-management perspective, the institution's approval matrix should heavily prioritize past credit reliability. Furthermore, the model's slight optimism (leaning toward false approvals) suggests that future iterations should incorporate threshold tuning to artificially make the model stricter, prioritizing the prevention of bad loans over the approval of good ones.

### Task 4: Medical Insurance Cost Prediction

- Objective: Build a regression model to accurately estimate medical insurance claim amounts based on personal demographic and lifestyle profiles.
- Technical Approach: Conducted EDA to identify linear relationships between demographics and medical costs. Transformed text-based categorical data into numerical formats. Trained a Linear Regression model and rigorously evaluated its predictive mapping using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
- Deep Business and Technical Insight: 
  - Identifying Cost Multipliers: While age and BMI showed expected positive correlations with medical costs, the analysis isolated Smoking Status as a massive, overriding cost multiplier. 
  - Strategic Impact: The higher RMSE in the model indicates the presence of extreme, unexpected medical outliers that standard linear models struggle to predict. However, the overwhelming weight of the smoking feature suggests that actuarial premium pricing models must strictly segment smokers into a distinct, high-cost risk pool. Failing to isolate this specific demographic would drastically skew baseline profitability for the insurance provider.

---

Thank you for reviewing my work. Please explore the individual project directories for detailed Jupyter Notebooks, and interactive visual deployments.
