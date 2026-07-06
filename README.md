# Wikipedia Web Traffic Forecasting

## Project Overview

This project develops an end-to-end time series forecasting pipeline to analyze and forecast Wikipedia web traffic across multiple languages.

The objective is to understand historical traffic patterns, identify trends and seasonality, and compare classical and advanced forecasting models for reliable traffic prediction.

## Dataset

The dataset contains daily page-view counts for Wikipedia pages across multiple languages and access channels.

The analysis includes:

- English
- Japanese
- German
- French
- Chinese
- Russian
- Spanish
- Wikimedia Commons
- MediaWiki

Page metadata such as language, access type, and access origin were extracted from the page identifiers before creating language-level time series.

## Project Workflow

The project follows the complete time series forecasting lifecycle:

1. Data loading and inspection
2. Metadata extraction
3. Data quality assessment
4. Exploratory data analysis
5. Missing value analysis and treatment
6. Language-level time series aggregation
7. Stationarity testing using the Augmented Dickey-Fuller (ADF) test
8. Baseline ARIMA modelling
9. ARIMA hyperparameter tuning
10. Baseline SARIMA modelling
11. SARIMA hyperparameter tuning
12. ARIMA vs SARIMA model comparison
13. ACF and PACF analysis
14. Time series decomposition
15. SARIMAX modelling with an exogenous campaign variable
16. Prophet modelling
17. Final model comparison and business recommendations

## Models Implemented

- ARIMA
- SARIMA
- SARIMAX
- Prophet

The models were evaluated using:

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- MAPE (Mean Absolute Percentage Error)

## Key Results

The project demonstrates that forecasting performance varies significantly across language-level traffic series.

For the English traffic series, the final tuned SARIMAX model achieved:

- **MAE:** 5.95 million page views
- **RMSE:** 7.94 million page views
- **MAPE:** 4.82%

The results also demonstrate the value of incorporating external campaign information through exogenous variables.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Scikit-learn
- Prophet
- Jupyter Notebook

## Business Applications

The forecasting pipeline can support:

- Website traffic planning
- Infrastructure and capacity planning
- Advertising allocation
- Campaign impact analysis
- Language-specific traffic strategy

## Repository Contents

- `wikipedia_traffic_forecasting.ipynb` — Complete end-to-end analysis and modelling notebook

## Author

**Veeranna Hanamashetti**

Data Science | Machine Learning | AI
