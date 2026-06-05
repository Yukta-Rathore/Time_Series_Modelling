# Time Series Forecasting of Household Energy Consumption

## Project Overview

This project focuses on **multivariate time series forecasting** of household electricity consumption using historical energy usage data. The objective is to predict future power consumption patterns by leveraging multiple correlated variables that influence household energy demand.

The project includes data preprocessing, exploratory data analysis, stationarity testing, feature engineering, model development, and forecast evaluation using multiple forecasting models.

---

## Dataset

The dataset used in this project is the **Individual Household Electric Power Consumption Dataset** from the UCI Machine Learning Repository.

**Dataset Link:**  
https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption

### Dataset Description

The dataset contains measurements of electric power consumption in a single household collected over nearly four years at one-minute intervals.

### Variables

| Variable              | Description                                                 |
|-----------------------|-------------------------------------------------------------|
| Date                  | Date of measurement                                         |
| Time                  | Time of measurement                                         |
| Global_active_power   | Household global minute-averaged active power (kilowatt)    |
| Global_reactive_power | Household global minute-averaged reactive power (kilowatt)  |
| Voltage               | Minute-averaged voltage (volts)                             |
| Global_intensity      | Household global minute-averaged current intensity (ampere) |
| Sub_metering_1        | Energy sub-metering for kitchen appliances (watt-hour)      |
| Sub_metering_2        | Energy sub-metering for laundry appliances (watt-hour)      |
| Sub_metering_3        | Energy sub-metering for climate control systems (watt-hour) |

---

## Problem Statement

Accurate forecasting of electricity consumption is crucial for:

- Energy demand planning
- Smart grid management
- Resource optimization
- Peak load reduction
- Efficient energy distribution

This project aims to forecast future household energy consumption using historical multivariate observations.

---

## Project Workflow

### 1. Data Preprocessing

- Handled missing values
- Combined date and time into a datetime index
- Performed feature engineering
- Resampled time series data
- Applied data scaling and normalization

### 2. Exploratory Data Analysis

- Trend analysis
- Seasonality detection
- Correlation analysis
- Consumption pattern visualization
- Distribution analysis

### 3. Statistical Testing

- Augmented Dickey-Fuller (ADF) Test
- Stationarity Analysis
- Granger Causality Tests
- Seasonal Decomposition

### 4. Forecasting Models

The following forecasting models were implemented and compared:

- SARIMA
- SARIMAX
- Holt-Winters Exponential Smoothing
- Vector AutoRegression (VAR)
- Prophet

### 5. Model Evaluation

Models were evaluated using:

- Mean Absolute Percentage Error (MAPE)
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

---

## Results

- Built an end-to-end forecasting pipeline on **2M+ records** of household energy consumption data.
- Predicted **Global Active Power** over a **60-day forecasting horizon**.
- Implemented and compared **5 forecasting models** with **6 exogenous variables**.
- Achieved a best performance of **0.44% MAPE** using **Prophet with exogenous regressors**.
- Reduced forecast error by approximately **98% compared to the univariate baseline model**.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels
- Prophet
- Scikit-learn

---

Data Science | Machine Learning | Time Series Forecasting
