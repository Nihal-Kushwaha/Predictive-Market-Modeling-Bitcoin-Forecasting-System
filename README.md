# 📈 Predictive Market Modeling: Bitcoin Forecasting System

## 🚀 Project Overview
This project is an advanced deep learning forecasting system built to predict the highly volatile price trajectory of Bitcoin. It evaluates and compares three distinct sequential neural network architectures to determine which model best captures long-term market dependencies:
* **SimpleRNN (Recurrent Neural Network)**
* **LSTM (Long Short-Term Memory)**
* **GRU (Gated Recurrent Unit)**

By leveraging 5 years of live market data via the `yfinance` API, the models process 60-day lookback windows to forecast the actual price of Bitcoin for the upcoming 7 days.

## 🛠️ Tech Stack
* **Programming Language:** Python
* **Deep Learning Framework:** TensorFlow / Keras
* **Data Processing & Scaling:** Pandas, NumPy, Scikit-Learn
* **Data Visualization:** Matplotlib
* **Financial Data API:** yfinance

## 📊 Key Findings & Results
After training all three models on the exact same dataset and parameters, the results clearly highlighted the internal differences of the architectures:
* **SimpleRNN:** Struggled significantly with the vanishing gradient problem. It failed to capture long-term market momentum and its future predictions degraded rapidly.
* **LSTM:** Successfully utilized its complex gating system (Forget, Input, Output gates) to remember historical context, providing highly accurate and stable predictions.
* **GRU:** Emerged as the most efficient model. It achieved the lowest Mean Absolute Error (MAE) and trained faster than the LSTM due to its streamlined architecture, while maintaining exceptional accuracy.

## 📈 Visualizations

### 1. Model Comparison on Historical Data
![Historical Comparison](https://github.com/Nihal-Kushwaha/Predictive-Market-Modeling-Bitcoin-Forecasting-System/blob/main/Historical%20Comparision.png)

### 2. 7-Day Future Forecast
![Future Forecast](https://github.com/Nihal-Kushwaha/Predictive-Market-Modeling-Bitcoin-Forecasting-System/blob/main/Future%20Forecast.png)



