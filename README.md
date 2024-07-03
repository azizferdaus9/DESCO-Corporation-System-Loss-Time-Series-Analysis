# DESCO-Corporation-System-Loss-Time-Series-Analysis

Project Overview

This project involves analyzing the system loss percentage of DESCO Corporation over a series of fiscal years. The goal is to understand past trends and forecast future system losses using various time series analysis techniques. The project includes simple linear regression, multiple linear regression, auto-regression, exponential smoothing, weighted moving average, and Holt-Winters exponential smoothing. Ultimately, we compare these models to identify the most accurate forecasting method.

Data Preparation

Loading Data:

Two datasets were used: one for simple linear regression and another for multiple linear regression, each containing fiscal year data and system loss percentages.
Data Cleaning:

Reversed the order of the fiscal year column.
Extracted the starting year from the fiscal year strings.
Converted system loss percentages from string to numeric format.
Time Series Analysis Methods

Simple Linear Regression (SLR):

Objective: Establish a linear relationship between fiscal years and system loss percentages.
Process: Split the data into features (fiscal years) and target variable (system loss %), fit a linear model, and forecast future values.
Evaluation Metrics: Root Mean Squared Error (RMSE), Mean Absolute Deviation (MAD), Mean Absolute Percentage Error (MAPE).
Multiple Linear Regression (MLR):

Objective: Use additional financial indicators (income, expense, profit/loss) to predict system loss percentages.
Process: Fit a linear model using multiple features and forecast future values.
Evaluation Metrics: RMSE, MAD, MAPE.
Auto-regression (AR):

Objective: Model the system loss percentage based on its own previous values.
Process: Fit auto-regressive models with different lags and select the best model based on evaluation metrics.
Evaluation Metrics: RMSE, MAD, MAPE.
Exponential Smoothing:

Objective: Apply exponential smoothing to the system loss percentages for forecasting.
Process: Use a smoothing parameter to give more weight to recent observations.
Evaluation Metrics: RMSE, MAD, MAPE.
Weighted Moving Average (WMA):

Objective: Use a weighted moving average to forecast future system loss percentages.
Process: Apply predefined weights to recent observations and calculate forecasted values.
Evaluation Metrics: RMSE, MAD, MAPE.
Holt-Winters Exponential Smoothing:

Objective: Use Holt-Winters exponential smoothing to capture seasonality and trends in the data.
Process: Fit the model and forecast future values.
Evaluation Metrics: RMSE, MAD, MAPE.
Results and Comparison

The performance of each model was evaluated using RMSE, MAD, and MAPE. The results were visualized using bar charts, showing the scores of each model:

RMSE Scores: Simple Linear Regression (0.88), Multiple Linear Regression (0.92), Auto-regression (0.42), Exponential Forecasting (0.43), Weighted Moving Average (0.54), Holt-Winter (0.52)
MAD Scores: Simple Linear Regression (0.69), Multiple Linear Regression (0.70), Auto-regression (0.35), Exponential Forecasting (0.36), Weighted Moving Average (0.46), Holt-Winter (0.42)
MAPE Scores: Simple Linear Regression (2.11%), Multiple Linear Regression (2.14%), Auto-regression (0.95%), Exponential Forecasting (0.98%), Weighted Moving Average (1.25%), Holt-Winter (1.20%)
Conclusion

Based on the comparison, Auto-regression emerged as the best model with the lowest RMSE, MAD, and MAPE scores. This suggests that auto-regression provides the most accurate forecasts for DESCO Corporation's system loss percentages among the models considered.

Visualization

For each model, actual vs. forecasted system loss percentages were visualized using line plots to provide a clear comparison of the forecasting performance. The bar chart summarizing the evaluation metrics highlighted the effectiveness of the auto-regression model.

Project Impact

This project demonstrates the application of various time series forecasting techniques in a real-world scenario. By identifying the most accurate model, DESCO Corporation can better predict and manage its system losses, leading to more informed strategic decisions.
