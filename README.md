# Stock-Portfolio-Optimization

This project focuses on optimizing a stock portfolio using Modern Portfolio Theory (MPT) and financial data sourced from Yahoo Finance. The analysis includes calculating risk-adjusted returns, constructing efficient frontiers, and enhancing portfolio performance through data-driven techniques.

## Features:

Historical Stock Data: Analyzed stock data from 2016-2021 using Yahoo Finance API.
Mean-Variance Optimization: Applied Mean-Variance Analysis to optimize portfolio weights, minimizing risk while maximizing returns.
Multilingual Approach: Utilized Python, R, and SQL for various stages of data extraction, transformation (ETL), and analysis.
Data Storage: PostgreSQL database to store historical stock data and results for performance tracking.
Performance Benchmarking: Compared the optimized portfolio’s performance against the S&P 500 index to demonstrate improvement.

## Getting Started

To run this project on your local machine:
Clone the repository:

git clone https://github.com/madhu-unnava/Stock-Portfolio-Optimization.git

Install dependencies: Follow the instructions in the setup_guide.md to install all required Python, R, and SQL dependencies.
Load data: Use the included scripts to fetch stock data from Yahoo Finance and load it into PostgreSQL.
Run the optimization: Execute the Python/R scripts to perform portfolio optimization and view the results.

All necessary code and datasets are included within the repository.

## Results
Annual Return: The optimized portfolio achieved an annual return of 38.39%, outperforming the S&P 500 index by 1.3x.
Risk-Adjusted Performance: By applying Modern Portfolio Theory, we reduced the portfolio's risk while maintaining strong returns, as visualized by the efficient frontier.

## Future Work
Incorporate real-time stock data for dynamic portfolio adjustment.
Explore other optimization models, such as Black-Litterman or Factor-Based models, for more sophisticated analysis.
