## Project Overview

The code follows these steps:

1. **Download Stock Data**  
   Fetches historical closing prices from Yahoo Finance using a specified stock symbol and date range.

2. **Visualize Historical Data**  
   Plots the historical closing price trend over time.

3. **Prepare Data for LSTM**  
   - Uses only the 'Close' column  
   - Scales the data to range [0, 1] using MinMaxScaler  
   - Creates input sequences of 60 time steps to predict the next day’s price

4. **Build and Train the Model**  
   - Sequential model with:  
     - Two LSTM layers (128 and 64 units)  
     - Two Dense layers (25 and 1 unit)  
   - Compiled with:  
     - Optimizer: Adam  
     - Loss: Mean Squared Error  
   - Trained for 10 epochs

5. **Make Predictions**  
   - Predicts future prices on test data  
   - Inverse-transforms predictions back to original price scale  
   - Calculates RMSE to measure prediction accuracy

6. **Visualize the Results**  
   - Plots training data, actual test values, and model predictions on the same chart  
   - Helps visually assess model performance

---

## How to Use

1. **Change the Stock Symbol**  
   In the code, modify this line:  
   ```python
   stock_symbol = 'AMZN'
   - Replace `'AMZN'` with any valid stock ticker (e.g., `'AAPL'`, `'GOOG'`, `'TSLA'`, `'NVDA'`).

1. **Run the Script**  
   Execute the code in your Python environment (Jupyter Notebook, VS Code, PyCharm, etc.).

2. **View Results**  
   You'll see:  
   - Training loss logs for each epoch  
   - RMSE value (lower = better)  
   - A plot comparing actual vs. predicted prices  

---

## Example Output  

- **Training Data Length:** ~95% of total data points  
- **RMSE Example:** ≈ 5.10 (USD)  
- **Plot Example:**  
  *(Actual plot will appear when you run the code)*
