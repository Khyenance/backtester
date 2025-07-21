#Stock Market Strategy Backtesting

## Project Overview
This project implements a basic moving average crossover strategy using Python. The strategy is applied to AAPL (Apple Inc.) stock data from 2020-01-01 to 2023-01-01, and benchmarked against a buy-and-hold market approach.
It uses basic technical analysis indicators such as the moving averages crossover to indicate a buy signal on AAPL using Python. The goal was to test if the moving averages crossover indicators were useful in outperforming the market

## Strategy Description
SMA10: 10 day simple moving average
SMA30: 30 day simple moving average

## Signal Logic
Buy signal when 10 day SMA10 > SMA30, otherwise no position
Signal is shifted 1 day before execution to avoid lookahead bias

## Technologies Used
- Python 3
- [yfinance](https://pypi.org/project/yfinance/) — for pulling historical stock data
- Pandas — for data manipulation
- NumPy — for numerical operations
- Matplotlib — for plotting strategy vs market performance
- Jupyter Notebook
- Git & GitHub

## Results
The strategy was backtested on AAPL from 2020-01-01 to 2023-01-01.
Performance was visualized using cumulative returns. While the strategy did generate signals and avoid some drawdowns, it underperformed the buy-and-hold market approach during strong bull runs.
<img width="556" height="437" alt="MarketOutperforms" src="https://github.com/user-attachments/assets/77eaf836-2525-4ed6-82b2-f6099f927518" />


## Future Improvements
-Add Sharpe Ratio, max drawdown
-Export results to CSV directly
-Add slippage and transaction costs into total returns
