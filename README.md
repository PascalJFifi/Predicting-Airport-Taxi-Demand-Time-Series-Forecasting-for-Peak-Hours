# Predicting Airport Taxi Demand: Time Series Forecasting for Peak Hours 🚕

Sweet Lift Taxi aims to improve driver availability during peak hours by forecasting taxi demand at airports. This project leverages historical data to build a predictive model that estimates the number of taxi orders for the next hour.

---

## 📝 Project Scope

The scope of this project involves analyzing historical taxi order data collected at airports to develop a predictive model for estimating demand in the next hour. Key aspects include:

* Resampling data to **hourly intervals**.
* Engineering time-based features such as **lags, rolling averages, and seasonal patterns**.
* Exploring forecasting techniques, including **Linear Regression, ARIMA, and ARMA**.
* Evaluating model performance using the **Root Mean Squared Error (RMSE)** metric, with a target threshold of **48**.

The final model will enable Sweet Lift Taxi to anticipate peak demand periods more accurately, allowing for better resource allocation and improved driver availability, ultimately enhancing overall service efficiency.

---

## 📂 Project Structure

The project is implemented in a Jupyter Notebook (`time_series_project.ipynb`) and includes the following main steps:

1.  **Data Preparation & EDA**:
    * Loading necessary Python packages.
    * Loading historical taxi order data from `taxi.csv`.
    * Setting the `datetime` column as the index and parsing it as datetime objects.
    * Sorting the data by the datetime index.
    * Displaying basic information about the dataset.
    * Resampling data to one-hour intervals by summing `sum_orders`.
2.  **Data Analysis**:
    * Analyzing the dataset for trends, seasonality, and potential missing values before model training.

---

## 🛠️ Libraries Used

This project utilizes the following Python libraries:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `statsmodels`
* `pmdarima`
* `scikit-learn` (specifically `LinearRegression`, `train_test_split`, `mean_squared_error`, `GridSearchCV`, `Ridge`, `StandardScaler`, `Pipeline`, `GradientBoostingRegressor`)
* `xgboost` (specifically `XGBRegressor`)

---

## 📊 Data

The historical taxi order data is stored in `taxi.csv`.

---

## 🎯 Goal

The primary goal is to build a time series forecasting model with an **RMSE score below 48** to predict taxi demand for the next hour at airports.
