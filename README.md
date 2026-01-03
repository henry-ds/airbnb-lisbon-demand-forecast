# Time Series Forecasting of Airbnb Demand in Lisbon

## Project Overview

This project analyzes and forecasts Airbnb demand in Lisbon, Portugal, using
monthly aggregated review data as a proxy for booking activity. The objective is
to explore temporal demand patterns and develop statistical forecasting models
capable of capturing trend and seasonality in a tourism-driven market.

The project follows a structured data science workflow, including data
preprocessing, exploratory time series analysis, and demand forecasting using
seasonal statistical models.

## Data Source

The raw dataset is obtained from the **Inside Airbnb** initiative, which provides
open-access data for research and policy analysis. The dataset contains individual
guest review records for Airbnb listings in Lisbon.

Due to its large size (~500MB), the raw dataset is processed locally and is not
included in this repository. Only aggregated and lightweight processed data are
stored to ensure reproducibility while respecting GitHub storage constraints.

## Methodology

The analysis is divided into three main stages, each documented in a separate
notebook:

### 1. Data Preprocessing
- Conversion of review timestamps to datetime format  
- Temporal aggregation of reviews at a monthly frequency  
- Construction of a time series representing monthly Airbnb demand  

### 2. Exploratory Time Series Analysis
- Visualization of long-term demand trends  
- Seasonal decomposition into trend, seasonal, and residual components  
- Identification of strong annual seasonality consistent with tourism patterns  

### 3. Demand Forecasting
- Train-test split with out-of-sample evaluation  
- Application of Seasonal ARIMA (SARIMA) models  
- Forecast evaluation using MAE and RMSE metrics  
- Visual comparison of forecasted and observed demand  

## Key Findings

- Airbnb demand in Lisbon exhibits strong annual seasonality, with peak activity
  during summer months.
- Seasonal decomposition confirms the presence of both long-term trends and
  regular seasonal patterns.
- SARIMA models effectively capture the seasonal structure of demand and provide
  reasonable short-term forecasts.

## Tools and Technologies

- Python  
- pandas, numpy  
- matplotlib, seaborn  
- statsmodels  
- scikit-learn  
- Jupyter Notebook  

## Notes on Reproducibility

The raw dataset is not included due to size constraints. Users may download the
Lisbon reviews dataset directly from the Inside Airbnb website and adjust file
paths in the preprocessing notebook if full replication is desired.

## Author

Anumba Emeka Henry
Aspiring MSc Data Science student 
