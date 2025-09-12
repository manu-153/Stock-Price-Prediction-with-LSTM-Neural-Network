# Stock-Price-Prediction-with-LSTM-Neural-Network

## Project Overview

This project focuses on forecasting stock prices by leveraging Long Short-Term Memory (LSTM) networks, a specialized type of recurrent neural network (RNN) well-suited for handling sequential and time-series data. By learning from patterns in historical stock market data, the model aims to generate reliable predictions of future price movements.

To demonstrate its effectiveness, the approach has been applied to the stock price data of four different companies, enabling comparative insights into model performance across varying market behaviors. This project highlights the practical application of deep learning in the domain of financial time-series forecasting, providing a foundation for further exploration into algorithmic trading, investment strategy development, and risk management.


___


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

This project uses LSTM networks to forecast stock prices. LSTM is a type of recurrent neural network (RNN) that is particularly well-suited for time series prediction tasks.

### Key Steps

1. **Data Retrieval**: Historical stock data is fetched for each company using the `yfinance` library.
   
2. **Data Preparation**:
   - Data is scaled using `MinMaxScaler`.
   - Training and testing datasets are created.
   - The LSTM model is trained on historical stock prices.

3. **Model Building**:
   - The model consists of two LSTM layers followed by dense layers.
   - It is compiled using the Adam optimizer & mean squared error loss function.

4. **Model Evaluation**:
   - Predictions are made for the testing dataset.
   - The model's performance is evaluated using RMSE (Root Mean Squared Error).

5. **Visualization**:
   - Historical and predicted stock prices are visualized.
   - Performance metrics and predictions are plotted.

## Results

* **Visualizations**:

  * The project outputs visual charts that compare actual historical stock prices with the model’s predicted prices for all four companies. These plots provide an intuitive view of how well the model tracks stock price movements and trends.
  * Additional graphs display the predicted closing prices alongside the actual values, highlighting the model’s ability to follow real market behavior.

* **Performance Metrics**:

  * The Root Mean Squared Error (RMSE) is computed for the predictions on the test dataset. This metric quantifies the average prediction error, serving as a key indicator of model accuracy.
  * RMSE scores for each company are presented and compared, offering a clear perspective on performance differences across the various stocks.

* **Historical Data and Predictions**:

  * For every company, both historical stock price data and the corresponding predicted values are displayed. This includes original records along with forecasted results, giving a comprehensive view of the model’s predictive strength.

---
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

