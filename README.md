# Stock Market Analysis for Tech Giants

## Project Overview and Purpose
This project provides a quantitative analysis of the "Big Tech" stocks (AAPL, GOOG, MSFT, AMZN) to evaluate their historical performance, volatility, and risk-return profiles. By utilizing financial visualization techniques and statistical methods, this project aims to provide data-driven insights for portfolio management and investment strategy.

## Key Technologies and Libraries
- **Language**: Python
- **Data Acquisition**: `yfinance` (Yahoo Finance API)
- **Data Manipulation**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`
- **Statistical Analysis**: `scipy`

## Methodology and Analysis Workflow
### 1. Data Collection & Visualization
- Real-time stock data was pulled using the `yfinance` library.
- **Trend Analysis**: Visualized adjusted closing prices and daily trading volumes to identify market trends.
- **Moving Averages**: Calculated and plotted 10-day, 20-day, and 50-day moving averages to smooth out price fluctuations and identify support/resistance levels.



### 2. Risk and Return Calculation
- **Daily Returns**: Calculated the percentage change in stock price day-over-day.
- **Correlation Analysis**: Used Seaborn heatmaps and `PairGrid` to determine how closely the price movements of different tech companies are tied to one another.
- **Value at Risk (VaR)**:
    - **Bootstrap Method**: Calculated the empirical quantiles of daily returns.
    - **Monte Carlo Method**: Simulated thousands of possible price pathways to estimate the maximum expected loss with a 95% confidence interval.



## Results and Insights
- **Risk-Reward Profile**: Generated scatter plots comparing the Expected Return vs. Standard Deviation (Risk) for each stock.
- **Correlation**: Found high positive correlations between major tech stocks, suggesting that these assets are often moved by similar macroeconomic factors.
- **Financial Stability**: Analysis of the "Cumulative Return" shows the long-term growth trajectory of an initial investment in each company.

## How to Run
1. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
