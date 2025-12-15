# Air Quality Forecasting Using Time-Series and Machine Learning Models

## Project Overview

This project focuses on forecasting daily concentrations of Carbon Monoxide (CO(GT)) and Nitrogen Dioxide (NO₂(GT)) using historical air-quality sensor data. Accurate short-term forecasting enables proactive air-quality management, supports public health decision-making, and helps mitigate exposure risks.

Multiple modeling approaches are implemented and compared, including statistical time-series models, machine learning regressors, and deep learning architectures, to identify the most effective forecasting strategy.

## Objectives

  - Clean and preprocess raw air-quality data
  
  - Analyze temporal trends and seasonality
  
  - Build forecasting models for CO and NO₂
  
  - Compare model performance using standard metrics
  
  - Visualize predictions and derive actionable insights

## Dataset Description

<img width="1559" height="220" alt="{630F2EE4-BD00-42CC-89B8-29E622F6ECA5}" src="https://github.com/user-attachments/assets/f1f81e87-7727-4485-b6fe-b1701a4e7821" />
Targets:

  - CO(GT) – Carbon Monoxide concentration
      
  - NO2(GT) – Nitrogen Dioxide concentration

Exogenous Variables

  - T – Temperature
      
  - RH – Relative Humidity
      
  - AH – Absolute Humidity

Preprocessing Notes

  - Missing values encoded as -200 were converted to NaN
      
  - Data was resampled to daily averages to improve stability and computational efficiency

## Project Workflow

  - Data Preprocessing
    
  - Datetime parsing and indexing
    
  - Numeric type conversion
    
  - Missing value imputation
    
  - Daily resampling

## Exploratory Data Analysis (EDA)

Purpose: Understand trends, variability, and seasonality.

📊 Plots shown here:

  - Time-series trend plots for CO(GT) and NO₂(GT)
    
  - Seasonality by day of week plots
    
  - Correlation heatmaps (if included)
## Feature Engineering

  - Lag features
    
  - Rolling statistics
    
  - Time-based features (weekday, month)

## Forecasting Models
  Models Implemented

  - ARIMA – Univariate statistical baseline
    
  - SARIMAX – Seasonal time-series model (weekly seasonality)
    
  - Ridge Regression – Linear ML baseline
    
  - Random Forest – Non-linear ensemble model
    
  - LSTM – Deep learning sequence model

## Model Evaluation

  Metrics Used

  - Mean Absolute Error (MAE)
    
  - Root Mean Squared Error (RMSE)
    
  - Mean Absolute Percentage Error (MAPE)

    <img width="1723" height="427" alt="{B81CB88E-7BA0-4859-8DF7-83161038F4FF}" src="https://github.com/user-attachments/assets/07c5715b-7828-438a-a483-62c733314f49" />
    <img width="1717" height="417" alt="{374C64DE-53F8-4B80-A994-3DD1A2464556}" src="https://github.com/user-attachments/assets/c0576b73-5e39-496e-a796-a8c4596d8b26" />

  📊 Plots shown here:

  - Actual vs Predicted plots (side-by-side for CO & NO₂)
    
  - Residual distributions

## Model Comparison (Key Section)

  Purpose: Identify the best performing model.

  📊 Plots shown here:

  - Bar charts comparing RMSE, MAE, and MAPE
    
  - Subplots comparing all models side-by-side
    
  - Overlay plots comparing best models

## Forecast Visualization

  📊 Plots shown here:

  - Future forecasts (7–30 days)
    
  - Historical vs forecasted values

# Final Model Recommendation
  <img width="509" height="330" alt="{74592204-C72E-45A5-8262-D3D219A42FE4}" src="https://github.com/user-attachments/assets/1c7dfcb8-33a4-4caa-9f62-56e130cb8711" />

## Technologies Used

  - Python
    
  - Pandas, NumPy
    
  - Matplotlib
    
  - Scikit-learn
    
  - tatsmodels
    
  - ensorFlow / Keras

