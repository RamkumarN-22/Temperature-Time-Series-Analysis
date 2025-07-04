# 🌡️ Temperature Time Series Analysis

## 📌 Project Overview

This project focuses on analyzing 5 years (1825 days) of temperature data for a specific city. The goal is to identify temperature trends, seasonal patterns, and generate a short-term forecast using time series modeling (ARIMA).

---

## 🧾 Problem Statement

Time-series datasets provide insights for applications such as:
- Forecasting weather and climate changes
- Studying natural phenomena
- Planning for energy, agriculture, and urban design

This dataset includes:
- Minimum, Maximum, and Average daily temperatures
- Sunrise and Sunset times

---

## 📂 Dataset Description

| Feature Name | Description |
|--------------|-------------|
| `DATE`       | Date of observation (2014–2018) |
| `MinTemp`    | Minimum temperature (°C) |
| `MaxTemp`    | Maximum temperature (°C) |
| `AvgTemp`    | Average temperature (°C) |
| `Sunrise`    | Time of sunrise (HHMM format as integer) |
| `Sunset`     | Time of sunset (HHMM format as integer) |

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Statsmodels (for ARIMA and decomposition)

---

## 📈 Project Workflow

1. **Data Cleaning**
   - Converted `DATE` to datetime
   - Handled missing values with forward fill
   - Converted sunrise/sunset to readable time format

2. **EDA (Exploratory Data Analysis)**
   - Time plots for Avg, Min, Max temperatures
   - Sunrise & Sunset patterns (optional)

3. **Time Series Decomposition**
   - Decomposed AvgTemp into trend, seasonality, and residuals

4. **Forecasting**
   - Applied ARIMA model to forecast average temperatures
   - Evaluated performance with RMSE and MAE

---

## 📌 How to Run

```bash
pip install pandas matplotlib seaborn statsmodels
