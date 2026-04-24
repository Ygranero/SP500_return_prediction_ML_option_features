# S&P 500 Return Prediction with Machine Learning & Option Market Data

Machine Learning pipeline to predict short-term S&P 500 returns using option market signals and time series modeling.

## Business Impact 
  - Improved predictive performance vs statistical models (ARIMA, GARCH).
  - Captured nonlinear relationships in financial markets using Machine Learning.
  - Demonstrated the predictive value of forward-looking option data.
  - Built a realistic forecasting framework.

## Problem
Short-term stock market predictions is notoriously difficult due to:
  - High noise
  - Nonlinearity
  - Regime changes


## Models Compared
|       Type         |           Models                 |
|--------------------|----------------------------------|
| Statistical        | Linear Regression, ARIMA, GARCH  |
| Machine Learning   | Random Forest, XGBoost           |


## Results
  - **Random Forest achieved best overall performance.**
  - ML models showed **lower prediction error** than statistical models.
  - **Volatility-based features (VIX, IV)** were strongest predictors.
  - Performance remained robust across **market regimes.**
    

## Insights
  - Financial markets contain **nonlinear patterns** → ML advantage.
  - Option market variables provide **forward-looking signals**.
  - Traditional models struggle in **high volatility periods**.
    

## Data
  - Source: Bloomberg
  - Period: 2019 - 2024
  - Frequency: Daily

### Features
  - Return lags (1d, 5d, 10d)
  - Trading volume
  - Put/Call ratio
  - Implied volatility (30d)
  - VIX & SKEW index
  - Yield curve slope (10Y - 3M US treasury bonds)

### Target:
  - 5-day forward return (log returns)


## Evaluation Metrics
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - Directional Accuracy
  - Diebold-Mariano test


## Explainability
  - Feature importance.
  - SHAP values


## Tech Stack
  - Python (pandas, numpy)
  - scikit-learn
  - xgboost
  - statsmodels
  - arch (GARCH)
  - matplotlib / seaborn
  - shap

## Author
Yared Granero
MSc in Applied Data Science for Banking and Finance
