# Task 2: Credit Risk Prediction

## Objective
To build a machine learning classification model capable of predicting whether a loan applicant is likely to default or be approved.

## Dataset
Loan Prediction Dataset (features include applicant income, loan amount, education status, and credit history).

## Approach
Data Cleaning: Addressed missing data by imputing median values for continuous numerical features and mode values for categorical text features.
Exploratory Data Analysis (EDA): Visualized the financial profiles of applicants using Seaborn histograms and count plots to understand income distributions and education levels.
  Feature Engineering: Converted categorical text variables into machine-readable numerical formats using One-Hot Encoding (`pd.get_dummies`).
  Modeling: Split the data (80/20) and trained a Logistic Regression classifier. Evaluated the model using an Accuracy Score and a Confusion Matrix.
  Advanced Explainability: Extracted and mapped model coefficients to generate a Feature Importance chart, providing transparent business insights into the algorithm's decision-making process.
  Live Interactive Deployment:Engineered an interactive GUI within the Colab environment utilizing Colab Forms. This feature acts as a diagnostic engine, allowing end-users to input custom financial parameters via sliders and receive real-time loan approval inferences and confidence scores without writing code.

## Results and Insights
Performance: The model achieved a robust baseline accuracy of 82.83%.
Key Business Driver: Through feature coefficient analysis, it was mathematically proven that `Credit_History` is the overwhelming primary driver for loan approvals in this dataset, drastically outweighing factors like raw income or loan amount.
