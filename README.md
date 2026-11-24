# Canadian Bank Performance and Risk Analysis

A Python and SQL analysis comparing the historical performance, volatility, drawdowns, correlations, and risk-adjusted returns of Canada's Big Six banks against the XFN Canadian financial-sector benchmark.

## Business Question

How have Canada's largest publicly traded banks compared in historical return, volatility, downside risk, and risk-adjusted performance relative to a Canadian financial-sector benchmark?

## Assets Analyzed

- Royal Bank of Canada
- Toronto-Dominion Bank
- Bank of Montreal
- Bank of Nova Scotia
- Canadian Imperial Bank of Commerce
- National Bank of Canada
- XFN iShares S&P/TSX Capped Financials Index ETF

## Analysis Period

January 2020 through November 2026.

## Tools

Python, pandas, NumPy, yfinance, matplotlib, seaborn, SQLite, SQL, Google Colab, and GitHub.

## Methods

- Collected adjusted market-price data using yfinance
- Checked missing values, duplicate dates, and invalid prices
- Calculated daily, monthly, cumulative, and annualized returns
- Measured annualized volatility and maximum drawdown
- Calculated Sharpe ratios using an assumed 3% risk-free rate
- Compared each bank with the XFN benchmark
- Analyzed daily-return correlations
- Stored analysis tables in SQLite
- Wrote five SQL queries for performance ranking, benchmark comparison, extreme losses, monthly extremes, and positive-day frequency

## Key Findings

- CIBC generated the highest cumulative and annualized returns.
- Royal Bank displayed the strongest overall risk-return balance, matching CIBC's Sharpe ratio with lower volatility and a smaller drawdown.
- National Bank generated strong returns but experienced the deepest maximum drawdown.
- Scotiabank underperformed XFN on annualized return and risk-adjusted performance.
- March 2020 was the worst month for every asset in the analysis.
- High correlations among the banks indicate limited protection against sector-wide shocks.

## Visualizations

![Cumulative Returns](figures/cumulative_returns.png)

![Risk and Return](figures/risk_return_scatter.png)

![Drawdown History](figures/drawdown_history.png)

![Return Correlations](figures/return_correlation_heatmap.png)

## Repository Structure

- `Canadian_Bank_Performance_and_Risk_Analysis.ipynb` — complete analysis
- `data/` — cleaned prices, returns, and summary metrics
- `database/` — SQLite analysis database
- `figures/` — exported visualizations
- `requirements.txt` — required Python packages

## Limitations

Historical performance does not predict future returns. Results depend on the selected period and a fixed 3% risk-free-rate assumption. The analysis excludes taxes, transaction costs, valuation ratios, bank fundamentals, and macroeconomic forecasts. XFN contains substantial exposure to the analyzed banks and is not a broad-market benchmark.

## Author

**Shyla Khullar**  
UBC Mathematics student pursuing a Statistics minor  
[LinkedIn](https://www.linkedin.com/in/shyla-khullar-a6a205247)

*This project is for educational purposes and is not investment advice.*
