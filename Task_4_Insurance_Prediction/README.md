# Task 4: Predicting Insurance Claim Amounts

## Objective
To estimate medical insurance claim amounts based on personal data using a machine learning model.

## Approach
Data Loading & Preparation: Loaded the Medical Cost Personal Dataset and converted categorical text variables (like smoking status and region) into numerical formats using one-hot encoding.
  Exploratory Data Analysis (EDA):** Generated scatter plots and box plots to visualize the relationships between age, BMI, smoking status, and total medical charges.
  Modeling: Split the data into training (80%) and testing (20%) sets and trained a Linear Regression model using `scikit-learn`.
  Evaluation: Tested the model's accuracy using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## Results and Insights
Key Insight: The EDA clearly showed that **smoking status** is the most significant factor driving up medical insurance charges, with age and BMI also showing positive correlations.
  Model Performance:Mean Absolute Error (MAE): ~$4,181
Root Mean Squared Error (RMSE): ~$5,796
Conclusion: The model successfully captures the general trend of medical costs. The higher RMSE indicates that while average predictions are fairly close, there are large outliers (likely extreme, unexpected medical events) that a standard linear model cannot perfectly predict.
