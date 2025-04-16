# 📈 Microsoft Stock Price Prediction Using LSTM

This project uses an LSTM (Long Short-Term Memory) neural network to predict Microsoft’s stock closing prices based on historical time-series data. It walks through data preprocessing, visualization, model training, and prediction, aiming to capture patterns in the stock’s price movement over time.

---

## 🧠 Project Overview

- **Data Source**: Microsoft stock historical data (`MicrosoftStock.csv`)
- **Goal**: Predict the closing stock price using previous 60-day windows
- **Model Type**: LSTM (Recurrent Neural Network)
- **Framework**: TensorFlow / Keras

---

## 📊 Data Analysis & Visualization

The project includes several visualizations to understand stock behavior:

- **Open vs. Close Prices Over Time**: Shows price trends
- **Trading Volume Over Time**: Highlights unusual spikes in activity
- **Correlation Heatmap**: Reveals relationships between numerical features
- **Close Price Trend (2013–2018)**: Focus period for modeling

---

## 🔄 Data Preparation

- Time-series data converted into supervised learning format using a 60-day rolling window
- Normalized using `StandardScaler` to improve model convergence
- Split into 95% training data and 5% testing data

---

## 🧪 Model Summary

- Two stacked LSTM layers for sequence learning
- A dense layer followed by dropout to reduce overfitting
- Final output layer to predict the next day’s closing price
- Compiled with Adam optimizer and evaluated using MAE and RMSE

---

## 📈 Results & Verdict

After training for 20 epochs, the model was able to:

- Track general trends in Microsoft’s stock price over time
- Produce predictions that closely follow real test data
- Maintain low prediction error (visually confirmed on plotted graphs)

### ✅ Verdict

The LSTM model demonstrates strong potential for predicting stock price trends, although like most time-series models, it may struggle with sudden, sharp price movements. It provides a solid baseline for further financial modeling and deep learning improvements.

---
