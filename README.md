# S&P 500 Return Prediction using Machine Learning and Option Market Features

This repository contains my Master's thesis roject focused on predicting short-term S&P 500 returns using Machine Learning models and option market data.

## Highlights
  - Developed and compared **Machine Learning models (Random Forest, XGBoost)** with **statistical models (ARIMA, GARCH, Linear Regression)**
  - Used **option market variables** (implied volatility, put/call ratio, SKEW index) as predictive features
  - Implemented **time-series cross-validation** to avpid look-ahead bias
  - Evaluated models using:
      - MAE, RMSE
      - Directional Accuracy
      - Diebold-MAriano test (statistical comparison of forecasts)
  - Performed **feature importance analysis using SHAP**

## Results
  - Machine learning models **outperformed statistical models**
  - Random Forest achieved the **best overall predictive performance**
  - Option-based variables (especially volatility measures) showed **better predictive power**
  - Performance remained robust across **different market regimes (low/high volatility)**

## Problem Statement
Short-term return prediction in financial markets is challenging due to noise and nonlinearity.
This project investigates whether **Machine Learning models combined with forward-looking option data** can improve predictive performance.

## Data
  - Source: Bloomberg
  - Period: 2019 - 2024
  - Frquency: Daily

### Features:
  - Return lags (1d, 5d, 10d)
  - Trading volume
  - Put/Call ratio
  - Implied volatility (30d)
  - VIX & SKEW index
  - Yield curve slope (10Y - 3M US treasury bonds)

### Target:
  - 5-day forward return (log returns)

## Models Implemented

### Benchmark Models
  - Linear Regression
  - ARIMA
  - GARCH (1,1)

### Machine Learning Models
  - Random Forest
  - -XGBoost

## Evaluation Metrics
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - Directional Accuracy
  - Diebold-Mariano test

## Model Interpretation
  - Feature importance (tree-based models)
  - SHAP valuea for explainability

## Tech Stack
  - Python
  - pandas, numpy
  - scikit-learn
  - xgboost
  - statsmodels
  - arch (GARCH)
  - matplotlib / seaborn
  - shap
