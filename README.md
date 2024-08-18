# Stock Price Prediction Using LSTM

## Project Overview

This project involves predicting stock prices using Long Short-Term Memory (LSTM) networks. The model has been applied to four different companies to forecast their future stock prices based on historical data.

## Companies Analyzed

- **Amazon.com, Inc. (AMZN)**
- **Apple Inc. (AAPL)**
- **Google LLC (GOOG)**
- **Microsoft Corporation (MSFT)**

## Project Details

### Data Collection

- **Data Source**: Yahoo Finance
- **Date Range**: From 2014-01-01 to the current date

### Model Overview

The project uses LSTM networks to forecast stock prices. LSTM is a type of recurrent neural network (RNN) that is particularly well-suited for time series prediction tasks.

### Key Steps

1. **Data Retrieval**: Historical stock data is fetched for each company using the `yfinance` library.
   
2. **Data Preparation**:
   - Data is scaled using `MinMaxScaler`.
   - Training and testing datasets are created.
   - The LSTM model is trained on historical stock prices.

3. **Model Building**:
   - The model consists of two LSTM layers followed by dense layers.
   - It is compiled using the Adam optimizer and mean squared error loss function.

4. **Model Evaluation**:
   - Predictions are made for the testing dataset.
   - The model's performance is evaluated using RMSE (Root Mean Squared Error).

5. **Visualization**:
   - Historical and predicted stock prices are visualized.
   - Performance metrics and predictions are plotted.

## Results

- **Visualizations**: 
  - The project's output includes visual plots comparing historical stock prices with predicted prices for each of the four companies. These plots help visualize the model's performance in capturing the trends and variations in stock prices.
  - Graphs of the model's predictions against the actual closing prices are generated, showing how closely the model's predictions align with real-world data.

- **Performance Metrics**:
  - The Root Mean Squared Error (RMSE) is calculated for the model's predictions on the test set. RMSE provides a measure of the average prediction error, helping to assess the model's accuracy.
  - RMSE values for each company are printed and compared, providing insights into the model's performance across different stocks.

- **Historical Data and Predictions**:
  - Historical stock price data and the model's predictions are printed for each company. This includes both the raw data and the forecasted values, offering a detailed view of the model's effectiveness.

## Future Improvements

- **Model Enhancements**:
  - Experiment with different LSTM architectures and hyperparameters (e.g., number of layers, units per layer, dropout rates) to potentially improve the model's performance.
  - Explore alternative deep learning models or hybrid approaches combining LSTM with other techniques such as attention mechanisms.

- **Feature Engineering**:
  - Incorporate additional features into the model, such as trading volume, technical indicators (e.g., moving averages, RSI), or macroeconomic factors, to enhance predictive accuracy.

- **Extended Analysis**:
  - Expand the analysis to include a broader range of companies or different asset classes (e.g., commodities, currencies) to test the model's generalizability.
  - Consider implementing a backtesting framework to evaluate the model's performance over different historical periods and market conditions.

- **Deployment**:
  - Develop a web or mobile application for real-time stock price predictions and visualizations.
  - Integrate the model with financial news sentiment analysis to potentially improve prediction accuracy based on current events.

