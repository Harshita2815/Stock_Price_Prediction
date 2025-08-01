## Maruti Suzuki Stock Price Forecasting using ARIMA and CNN-LSTM

This project focuses on time series forecasting of Maruti Suzuki stock prices using both classical statistical methods (ARIMA) and a deep learning-based hybrid approach (1D CNN-LSTM). It includes exploratory data analysis, preprocessing, model building, evaluation, and visualization.

#### Tools & Libraries Used:

Python

Pandas, NumPy — Data manipulation

Matplotlib, Plotly, Seaborn — Data visualization

Statsmodels — ARIMA modeling

Scikit-learn — Evaluation metrics

TensorFlow / Keras — Deep learning (CNN-LSTM)

#### Exploratory Data Analysis (EDA):

Plotted OHLC, Volume, VWAP

Monthly & annual average prices

Visualized candlestick charts

Identified seasonality, trend, and volatility

Applied log transformation for stabilization of variance

#### ARIMA Modeling (Baseline):

STL decomposition used to analyze seasonal and trend components

Checked stationarity using ADF test

Applied differencing, and plotted ACF & PACF

Tried various models: ARIMA(0,1,0), ARIMA(1,1,0), ARIMA(0,1,1)

Selected model using AIC/BIC criteria

#### ARIMA Evaluation (Last 30 Business Days):

Forecasted stock prices for 30 days

MAPE: 1.38%

Actual vs Predicted plotted with 95% confidence intervals

#### Deep Learning: 1D CNN + LSTM Model:

Model:
Input Layer
→ 1D Convolutional Layer
→ MaxPooling
→ LSTM Layer
→ Dense Layer (Output)


##### Model Evaluation:

MSE: 1,020,594.91

MAE: 851.16

R² Score: 0.2375

Adjusted R²: 0.1999

#### Actual vs Predicted (CNN-LSTM):

Plotted side-by-side predictions vs actual for test period.

📅 Data Used
Source: [NSE/BSE or Kaggle]

Time Range: 2003-07-09 to 2020-10-30

#### How to Run:
Clone this repository

Install dependencies from requirements.txt

Run arima_model.ipynb for statistical modeling

Run cnn_lstm_model.ipynb for deep learning approach

Visualizations are saved in /results/plots

#### Future Work:
Hyperparameter tuning of CNN-LSTM using KerasTuner

Try Transformer models or Hybrid Prophet-ARIMA

Deploy forecast as a Streamlit dashboard

