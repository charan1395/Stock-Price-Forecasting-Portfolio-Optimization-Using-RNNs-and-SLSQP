**Stock Price Forecasting & Portfolio Optimization Using RNNs and SLSQP**
🧠 Overview
This project combines deep learning and financial modeling to build an end-to-end stock price forecasting and portfolio optimization pipeline. Using 20 years of historical data from five uncorrelated Dow Jones stocks, we forecast future stock returns with LSTM-based RNNs and apply Sharpe Ratio-based optimization via Sequential Least Squares Programming (SLSQP) to allocate portfolio weights that maximize risk-adjusted returns.

-----
💡 Objectives
Forecast future stock prices using LSTM-based RNN models.

Rebalance the portfolio yearly while accounting for withdrawals.

Maximize the Sharpe ratio by optimizing portfolio weights using SLSQP.

Evaluate portfolio survival under different withdrawal strategies.

Demonstrate the value of deep learning for long-term investment strategies.

-----
📊 Dataset
Source: Yahoo Finance via yfinance

Stocks Used: Microsoft (MSFT), Coca-Cola (KO), Johnson & Johnson (JNJ), 3M (MMM), Exxon Mobil (XOM)

Duration: 20 years of historical daily data

Criteria: Selected based on low inter-stock correlation to ensure diversification.

-----
🛠️ Technologies Used
Python

Pandas, NumPy, yfinance

TensorFlow / Keras for LSTM models

Optuna for hyperparameter tuning

Scikit-learn

Matplotlib, Seaborn for visualization

SciPy (SLSQP) for portfolio optimization

-----
🔁 Methodology
Data Collection: Fetched 20 years of historical price data.

Preprocessing: Cleaned, scaled, and transformed data for modeling.

Forecasting with LSTM: Built and tuned LSTM models for each stock using Optuna.

Portfolio Optimization:

Rebalanced annually with equal weights.

Applied SLSQP to maximize Sharpe ratio after each forecast cycle.

Survival Analysis: Simulated withdrawal scenarios and tracked portfolio sustainability.

-----
📈 Key Results
Achieved 62% reduction in RMSE through LSTM tuning.

Reduced MAPE to 1.11%, improving forecast accuracy.

Identified optimal portfolio allocation that balances growth and risk.

Built an explainable and adaptable framework for long-term portfolio strategy.

-----
🧠 Business Impact
This project provides a scalable solution for financial advisors and asset managers to forecast stock behavior and strategically rebalance portfolios. The methodology can be adapted for robo-advisors or retirement fund planning, offering intelligent, data-driven decisions that improve investor confidence and returns.
