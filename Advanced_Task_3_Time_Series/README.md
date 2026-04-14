Task 3: Energy Consumption Time Series Forecasting
Objective

To forecast short-term household energy usage using historical time-based patterns and compare the predictive accuracy of classical statistical models against modern machine learning algorithms.
Dataset

Household Power Consumption Dataset, resampled to daily frequencies to analyze long-term seasonal and weekly trends.
Approach

    Data Engineering: Cleaned historical data using forward-fill imputation for missing days. Engineered specific time-based features including month, day of the week, and binary weekend indicators.

    Machine Learning (XGBoost): Trained a tree-based XGBRegressor using the engineered time clues to capture human behavioral spikes.

    Advanced Forecasting (Prophet): Deployed Meta's Prophet algorithm, tuning it to specifically look for overlapping weekly and yearly seasonalities.

    Classical Statistics (ARIMA): Applied a traditional AutoRegressive Integrated Moving Average model as a mathematical baseline.

    Evaluation: Scored all models using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE), and visualized the predictions against actual historical usage using Matplotlib.

Results and Business Insights

    Prophet emerged as the superior forecasting engine (MAE: 86.79), slightly edging out XGBoost (MAE: 92.00) and drastically outperforming the classical ARIMA model (MAE: 176.81).

    Strategic Impact: The failure of ARIMA highlights that traditional statistics are insufficient for modern utility grids. By deploying Prophet, energy providers can highly optimize power distribution based on highly accurate, automated predictions of human behavioral patterns (e.g., weekend and winter usage spikes), minimizing both grid overload risks and wasted energy production.
