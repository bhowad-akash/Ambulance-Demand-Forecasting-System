# Jakarta Ambulance Demand Forecasting System
## Overview
This project develops a sophisticated time series forecasting system using real-world data from Jakarta to predict daily ambulance call volumes. The goal is to optimize emergency service planning and resource allocation by accurately forecasting future demand.
## Features
To capture the dynamics of the call volumes, a comprehensive range of time series forecasting models were implemented.
* **Baseline Model:** Utilizes Naive and Moving Average techniques to establish initial forecasting benchmarks.
* **Intermediate Models:** Employs Holt’s Linear and ARIMA models to enhance prediction accuracy over baseline models.
* **Advanced Models:** Implements Holt-Winters and SARIMAX models to capture seasonal trends and autocorrelation for precise rolling forecasts.
## Data
The dataset comprises ambulance call data for 3 Months, including:

* **Total calls:** 32,905<br/>
* **Average calls per day:** 153<br/>
* **Standard deviation:** 37.42<br/>
* **Most active calling hour:** 10:00 AM<br/>

Key insights include variability in daily call volumes, peak calling times, and weekly cycles.
## Methodology
### Preprocessing
* **Date Conversion:** Converting call dates to datetime format.
* **Feature Extraction:** Deriving features such as hour, day of the week, and month.
* **Summary Statistics:** Calculating and visualizing descriptive statistics and call volumes.
### Models
* **Baseline Models:** Naive, Moving Average
* **Exponential Smoothing Models:** Simple Exponential Smoothing, Holt’s Linear, Holt-Winters
* **Regression Model:** Simple Linear Regression
* **ARIMA Models:** ARIMA, SARIMA

Stationarity tests (ADF and KPSS) and decomposition plots were used to analyze and prepare the data for modeling.
### Performance Metrics
Models were rigorously evaluated using metrics such as:

* **Mean Squared Error (MSE)**
* **Mean Absolute Percentage Error (MAPE)**

The SARIMA model achieved the best performance with:

* **MSE:** 202
* **MAPE:** 7.15%
## Technologies Used
* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Statsmodels**
* **scikit-learn**
## Contributing
Contributions to enhance the forecasting models or extend the dataset are welcome. Please follow these steps:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.
## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
