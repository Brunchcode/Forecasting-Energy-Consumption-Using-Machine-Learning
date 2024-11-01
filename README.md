# Forecasting Energy Consumption Using Machine Learning
## Msc Data Science Distertation 
### Distinction

This project focuses on forecasting energy consumption using machine learning models, developed as part of an MSc dissertation at Manchester Metropolitan University. This project aims to improve the accuracy of short-term and long-term energy consumption forecasts, addressing limitations in traditional methods and supporting efficient energy management towards net-zero goals.

## Project Overview

Energy demand is rising, with patterns becoming increasingly complex and nonlinear. Traditional forecasting methods often struggle to capture these complexities, resulting in inaccuracies. This project leverages historical data from the PJM Interconnection (Dominion Energy) to create a series of machine learning models, including linear regression, decision trees, random forests, gradient boosting, and neural networks (MLP, CNN, LSTM), to forecast energy consumption more accurately.

## Table of Contents

- [Data](#data)
- [Methodology](#methodology)
- [Models Used](#models-used)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Key Findings](#key-findings)
- [Conclusion](#conclusion)
- [Acknowledgements](#acknowledgements)

## Data

The dataset used in this project comes from the PJM Interconnection (Dominion Energy) covering energy consumption data from 2006 to 2024. Key variables include:
- **Energy Consumption** in MW
- **Temperature** and other weather-related variables
- **Date and Time** to allow for time-series modeling

Data preprocessing steps included handling missing values, normalizing data, and feature engineering, such as creating datetime and weather-related features.

## Methodology

1. **Data Preprocessing:** Data was transformed to a time-series format, missing values were handled, outliers were managed, and data normalization was applied.
2. **Model Development:** A range of machine learning models were implemented, including:
   - Linear Regression
   - Decision Tree
   - Random Forest Regressor
   - Gradient Boosting Machine (GBM)
   - Extreme Gradient Boosting (XGBoost)
   - Support Vector Regression (SVR)
   - Neural Networks (MLP, CNN, LSTM)
3. **Hyperparameter Tuning:** Performed to optimize each model’s performance.
4. **Model Explainability:** Feature importance was analyzed using SHAP (SHapley Additive exPlanations) to interpret model predictions.

## Models Used

- **Linear Regression**: Basic model for baseline performance.
- **Decision Tree**: Simplistic model that splits data based on decision nodes.
- **Random Forest**: An ensemble of decision trees that improves prediction stability.
- **Gradient Boosting**: Iteratively builds models to correct errors of previous models.
- **XGBoost**: Optimized gradient boosting with higher accuracy and computational efficiency.
- **Neural Networks**: MLP, CNN, and LSTM were used for capturing complex relationships.

## Evaluation Metrics

Each model was evaluated using the following metrics:
- **RMSE**: Root Mean Squared Error
- **MAE**: Mean Absolute Error
- **MAPE**: Mean Absolute Percentage Error

## Results

The top-performing models were:
1. **LSTM (Long Short-Term Memory)**: Excelled in capturing temporal dependencies in time-series data.
2. **Ensemble Model (XGBoost + Random Forest + Gradient Boosting)**: Combined models for higher accuracy.
3. **Tuned XGBoost**: Optimized model achieving a balance of accuracy and computational efficiency.

These models demonstrated significant improvements in forecast accuracy compared to traditional methods.

## Key Findings

- **Feature Importance**: SHAP analysis highlighted temperature and time-of-day as influential factors.
- **Model Performance**: Machine learning models, especially LSTM, outperformed traditional forecasting methods.
- **Practical Implications**: Enhanced forecast accuracy supports more efficient energy management and sustainable energy practices.

## Conclusion

This study shows the effectiveness of machine learning models in forecasting energy consumption, with neural networks, especially LSTM, providing the best performance. These findings support the integration of machine learning in energy management systems and contribute to the broader goal of achieving net-zero energy consumption.

## Acknowledgements

Special thanks to my supervisor and the GEM – Portfolio Optimisation team at ScottishPower for their guidance, and to Manchester Metropolitan University for the resources and support.

