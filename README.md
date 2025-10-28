# 📊 Stock Market Trend Prediction using Prophet & Yahoo Finance

This project demonstrates how to **analyze, visualize, and forecast stock market data** using Python libraries such as **yfinance**, **Prophet**, and **Plotly**.
It fetches real-time stock data, cleans and processes it, and then predicts future stock trends for the next 7 days.

---

## 🚀 Features

✅ Fetches real-time stock data from **Yahoo Finance** using `yfinance`
✅ Cleans and processes stock data (Moving Averages, Daily Returns, etc.)
✅ Predicts **future stock prices** using Facebook’s **Prophet** model
✅ Visualizes **actual vs predicted** prices using interactive **Plotly** charts
✅ Highlights the **next 7 days of forecasted prices**

---

## 📦 Installation

1. Clone this repository

   ```bash
   git clone https://github.com/yourusername/stock-market-forecast.git
   cd stock-market-forecast
   ```

2. Install the required libraries

   ```bash
   pip install yfinance pandas numpy scikit-learn prophet plotly
   ```

---

## 🧠 Libraries Used

| Library        | Purpose                                 |
| -------------- | --------------------------------------- |
| `yfinance`     | Fetch financial data from Yahoo Finance |
| `pandas`       | Data manipulation and cleaning          |
| `numpy`        | Numerical operations                    |
| `scikit-learn` | Machine learning utilities              |
| `prophet`      | Time series forecasting                 |
| `plotly`       | Interactive data visualization          |

---

## 📈 Usage

1. **Run the script** to fetch and clean stock data:

   ```python
   df = fetch_stock_data('AAPL')
   df = process_stock_data(df)
   ```

2. **Generate forecast** for the next 7 days:

   ```python
   forecast = predict_trend(df)
   ```

3. **Visualize results**:

   ```python
   fig.show()
   ```

You can change the stock ticker (e.g., `'TSLA'`, `'MSFT'`, `'GOOG'`) inside the function:

```python
df = fetch_stock_data('TSLA')
```

---

## 📊 Example Output

* **Data Processing:**
  Calculates 10-day and 30-day moving averages
  Computes daily return percentage
  Cleans missing and invalid values

* **Forecast Example:**

  | Date       | Predicted Price | Lower Limit | Upper Limit |
  | ---------- | --------------- | ----------- | ----------- |
  | 2025-10-25 | 187.12          | 184.55      | 189.44      |
  | 2025-10-26 | 188.22          | 185.00      | 190.50      |
  | 2025-10-27 | 189.10          | 186.02      | 192.00      |

---

## 📉 Visualization

An interactive Plotly chart showing:

* Actual closing prices
* Forecasted future prices
* Highlighted future 7-day prediction region

---

## 🧩 File Structure

```
📁 stock-market-forecast/
│
├── stock_forecast.py        # Main Python script
├── README.md                # Project documentation
└── requirements.txt         # Required libraries (optional)
```

---

## 🧠 Future Enhancements

* Add more technical indicators (RSI, MACD)
* Include multiple stock tickers in one visualization
* Build a small dashboard using **Streamlit**

