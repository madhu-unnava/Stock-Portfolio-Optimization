💼 Mean-Variance Portfolio Optimization

This project centers around optimizing a portfolio of 15 selected stocks using the Mean-Variance (Markowitz) Portfolio Optimization method. The goal is to minimize risk while maximizing returns by analyzing historical stock data. The stock data spans from December 31, 2015, to March 26, 2021, and performance is evaluated against the S&P 500 Total Return (SP500TR) index.

📝 Project Overview

This project follows an ETL (Extract, Transform, Load) process to extract and prepare stock market data from Yahoo Finance. The Mean-Variance Optimization (MV) technique is applied to create a portfolio that achieves an optimal balance between risk and return. The focus is on analyzing stock performance from 2016 to 2020, with a back-test on 2021 performance.

Key Objectives:
Data ETL: Perform data extraction, transformation, and loading using PostgreSQL and SQL for stock data integration.
Portfolio Optimization: Apply Mean-Variance portfolio optimization to assign optimal weights to the stocks.
Performance Evaluation: Compare the optimized portfolio against the SP500TR index.
Risk-Return Analysis: Evaluate the risk and return metrics of the optimized portfolio versus the benchmark.
📊 Data Summary

Source: Stock data was retrieved from Yahoo Finance for 15 selected stocks, along with the S&P 500 index.
Period: Data covers December 31, 2015, to March 26, 2021, for portfolio optimization and analysis.
Key Stocks:
CCBC, CRWS, CME, JAZZ, JPM-PD, JXHLY, NVZMF, NILSY, NKSH, SQBG, STLD, SEB, USLM, UNB, USNU 

🧑‍💻 Methodology

ETL Process:
Extraction: The stock prices and S&P 500 data were sourced from Yahoo Finance and integrated into a PostgreSQL database.
Transformation: Data was cleaned and transformed, including creating a custom trading calendar and handling missing values. A pivot table was used to reshape the data for further analysis.
Loading: Cleaned and transformed data was loaded into the analysis pipeline for portfolio optimization.
Mean-Variance Portfolio Optimization:
Markowitz Model: This model optimizes the portfolio by minimizing risk (variance) while targeting a specific return based on the S&P 500 index.
Training & Testing Split: Data from 2016 to 2020 was used for training, while data from the first 58 trading days of 2021 was used for back-testing.
Portfolio Weights: Optimized weights were assigned to the stocks. Some stocks were shorted (assigned negative weights) as part of the optimization.
📈 Results

Cumulative Returns:
2016-2020: The cumulative return analysis showed that certain stocks like STLD performed exceptionally well, with a positive return of 181%. On the other hand, CRWS had the lowest return at -9.5%.
2021 Performance: The portfolio achieved an annualized return of 38.39%, outperforming the SP500TR, though it had slightly higher risk due to a larger standard deviation.
Key Metrics:
Annualized Return: Portfolio: 38.39%, S&P 500: 29.87%
Annualized Standard Deviation: Portfolio: 15.56%, S&P 500: 16.23%
Sharpe Ratio: Portfolio: 2.47, S&P 500: 1.84 (higher Sharpe ratio indicates better risk-adjusted returns)
📊 Visualization and Insights

Cumulative Return Charts: A comparison of portfolio performance vs. the S&P 500 showed that the portfolio outperformed the index with a cumulative return of 155%, compared to the SP500TR’s 115%.
Portfolio Weights: JPM-PD had the highest weight (40.63%), while NKSH and SQBG had negative weights, indicating short positions.
🛠️ Recommendations

Risk Management: While the portfolio shows high returns, it comes with increased risk. Investors may consider balancing high-risk stocks with more stable assets.
Stock Selection: Adding stocks with higher liquidity or diversification could further reduce risk.
Rebalancing: Regularly rebalancing the portfolio based on market conditions is advised to maintain optimal risk-return balance.
🚀 Future Work

Advanced Optimization: Exploring techniques like Black Litterman or Hierarchical Risk Parity (HRP) could improve the portfolio’s performance.
Factor Models: Incorporating factor models (e.g., Fama-French) for stock selection may lead to better portfolio returns.
Extended Backtesting: Backtesting over a longer period could help validate the robustness of the optimization model.
