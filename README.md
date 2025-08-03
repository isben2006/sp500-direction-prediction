# S&P 500 Daily Direction Prediction

## Project Overview
This project aims to predict whether the S&P 500 index will close higher or lower the next day using supervised machine learning techniques. The prediction is based on historical price data and a set of technical features derived from it.

## Data Source
- **Ticker:** ^GSPC (S&P 500 Index)  
- **Data Provider:** Yahoo Finance via `yfinance` Python library  
- **Period:** January 1, 2020 – July 31, 2025


## Features Used
| Feature Name           | Description                                      | Lookback Window (days)  |
|-----------------------|------------------------------------------------|------------------------|
| Daily Return          | Percentage price change from previous day       | 1                      |
| 5-day Moving Average  | Average close price over the past 5 days        | 5                      |
| 10-day Moving Average | Average close price over the past 10 days       | 10                     |
| Momentum (5-day)      | Difference between today’s and 5 days ago close | 5                      |
| Rolling Std Dev (10-day) | Standard deviation of close prices over 10 days | 10                     |
| Average True Range (ATR) | Measure of volatility over 14 days             | 14                     |
| Relative Strength Index (RSI) | Momentum oscillator over 14 days           | 14                     |
| Lagged Return (1-day) | Previous day’s return                            | 1                      |
| MACD                  | Moving Average Convergence Divergence indicator | 26 (slow EMA)  |

## Next Steps
- Download historical data and compute features.  
- Prepare the dataset for supervised learning by handling missing values and creating the target variable.  
- Train and evaluate classification models such as logistic regression.  
- Analyze results and iterate on feature engineering and model tuning.

## How to Run
1. Clone this repository.
2. Install the required Python packages (e.g., `yfinance`, `pandas`, `ta`, `scikit-learn`).
3. Run the provided Python scripts to download data, compute features, and train models.

## License
This project is open-source and free to use.

---

