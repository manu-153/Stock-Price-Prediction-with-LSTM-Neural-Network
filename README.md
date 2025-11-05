# Stock Price Prediction using LSTM
This project uses a Long Short-Term Memory (LSTM) neural network to predict stock prices based on historical closing data.
It downloads stock data using Yahoo Finance, trains a model, and visualizes both actual and predicted prices.

## 📦 Requirements
Make sure you have the following libraries installed:
bashDownloadCopy codepip install yfinance numpy pandas matplotlib scikit-learn keras tensorflow

## 📁 Project Overview
Steps in the code:

1. 
Download Stock Data

Fetches data from Yahoo Finance using the stock symbol (e.g., AMZN).
Uses a specified date range.


2. 
Visualize Historical Data

Plots the historical closing prices.


3. 
Prepare Data for LSTM

Uses only the “Close” column.
Scales the data between 0 and 1 using MinMaxScaler.
Creates training sequences with 60 time steps.


4. 
Build and Train the Model

A Sequential model with two LSTM layers and Dense output layers.
Compiled with Adam optimizer and Mean Squared Error loss.
Trains for 10 epochs.


5. 
Make Predictions

Predicts future prices on test data.
Scales predictions back to original prices.
Calculates RMSE (Root Mean Squared Error).


6. 
Visualize the Results

Compares real vs. predicted closing prices.
Plots them together for evaluation.




## 🧩 How to Use

1. 
Change the Stock Symbol:
In the code, modify this line:
pythonDownloadCopy codestock_symbol = 'AMZN'
Replace 'AMZN' with any valid ticker (e.g., 'AAPL', 'GOOG', 'TSLA', etc.).

2. 
Run the Script:
Run it in your Python environment (e.g., Jupyter Notebook or any IDE).

3. 
View Results:

You’ll see:

A training loss log
RMSE value
Graph showing actual vs. predicted stock prices






## 📊 Example Output

* Training Data Length: ~95% of dataset
* RMSE Example: ≈ 5.10
* Plot Example:
Compares model predictions with real data for validation.


## ⚙️ Notes

* You can increase the number of epochs to improve accuracy.
* LSTM performance may vary between stocks — try retraining for each one.
* The dataset automatically updates with the latest stock data when you run the code.
