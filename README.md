# LLM-Performance-Evaluation-for-Price-Prediction-in-Crypto-Stocks
This project aims to compare the performance of various open-source Large Language Models (LLMs) in predicting the price movements of cryptocurrencies and stocks. The goal is to assess how well these models handle price prediction tasks in financial markets with different levels of volatility, such as cryptocurrencies and traditional stocks.
# Project Overview
The project explores the use of open-source LLMs (like GPT-based models) to predict price movements and evaluates their performance against the backdrop of highly volatile cryptocurrencies and relatively stable stock markets.

## Objective: To determine which open-source LLM provides the best performance in predicting cryptocurrency and stock prices.
## Scope: Fine-tuning and testing of different LLMs for both cryptocurrency and stock price forecasting, followed by a comparative analysis of their performances.
# Features
## Data Sources:

### Cryptocurrency Data: Collected using the ccxt library from major exchanges (e.g., Kraken).
### Stock Data: Collected using yfinance for stocks like Apple (AAPL) and Tesla (TSLA).
## LLMs Used:

GPT-2 and other open-source models from the Hugging Face transformers library.
## Data Preprocessing:

Data normalization and scaling for both cryptocurrencies and stocks.
Feature engineering, including moving averages and volatility calculations.
## Modeling:

Fine-tuning various LLMs for time series prediction by converting OHLCV (Open, High, Low, Close, Volume) data into sequences suitable for LLMs.
Evaluating performance across different time periods and assets.
## Evaluation:

Comparative analysis of the LLMs’ performances on stocks and cryptocurrencies.
Metrics: Mean Squared Error (MSE), training loss, and visualization of predicted vs actual prices.

# Project Structure
## Data Collection:
ccxt is used to fetch cryptocurrency data (e.g., Bitcoin and Ethereum).
yfinance is used to collect stock data (e.g., Apple, Tesla).
## Preprocessing:
Data cleaning, normalization using MinMaxScaler, and missing value handling via forward/backward filling.
## LLM Fine-Tuning:
LLMs from Hugging Face are fine-tuned on the OHLCV data, treating historical price data as sequences for prediction.
## Evaluation:
Each LLM is evaluated based on its ability to predict future prices with MSE as the primary evaluation metric.

# Requirements
Python 3.x
TensorFlow or PyTorch (depending on the model)
Hugging Face transformers
ccxt (for cryptocurrency data)
yfinance (for stock data)
pandas, numpy, and scikit-learn (for preprocessing)







