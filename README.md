# Axis Flexi Cap Fund NAV Forecasting using Time-Series Analysis

## Project Overview

This project focuses on analysing and forecasting the Net Asset Value (NAV) of the Axis Flexi Cap Fund (Direct Plan – Growth) using Python-based time-series analysis. The objective was to understand historical NAV movements, examine underlying trends and patterns, compare forecasting techniques, and identify the model most suitable for short-term NAV prediction.

## Dataset

The analysis used 990 daily NAV observations covering the period from 1 September 2022 to 26 August 2026. Data preprocessing involved date formatting, chronological sorting, duplicate and missing-value checks, and handling non-trading days to create a continuous time series.

## Methodology

**1. Exploratory Data Analysis (EDA):** Examined historical NAV trends, daily returns, moving averages, volatility, seasonality, and autocorrelation using visualisations and statistical analysis.

**2. Stationarity Testing:** Applied the Augmented Dickey-Fuller (ADF) test to assess stationarity. Log transformation and first differencing were used to make the series suitable for statistical forecasting.

**3. Model Development:** Developed and compared four forecasting approaches:
- Naive Forecast
- 10-Day Moving Average
- Holt’s Exponential Smoothing
- ARIMA

**4. Model Evaluation:** Reserved the final 90 observations for testing and evaluated forecast accuracy using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE). Residual diagnostics, including the Ljung-Box test, were used to assess the selected model.

## Key Results

Holt’s Exponential Smoothing outperformed the other evaluated models, achieving a test MAPE of **2.76%**. The model was subsequently used to generate a 30-trading-day NAV forecast. A comparison with a publicly reported NAV value for 3 September 2026 showed a forecast difference of ₹0.26, or approximately 0.82%.

## Technologies Used

Python, Pandas, NumPy, Matplotlib, Statsmodels, Time-Series Analysis, Statistical Testing, and Forecast Evaluation.

## Conclusion

The project demonstrates an end-to-end approach to financial time-series forecasting, combining data preparation, statistical testing, model comparison, and residual diagnostics. The results highlight the importance of model validation and the limitations of forecasts based solely on historical NAV data. The forecasts are analytical estimates and should not be interpreted as investment advice.
