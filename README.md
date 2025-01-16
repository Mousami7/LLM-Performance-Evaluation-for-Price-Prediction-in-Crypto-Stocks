
![Thesis](https://github.com/user-attachments/assets/24d18849-77db-40c6-a74c-61ed8e896525)


# LLM-Performance-Evaluation-for-Price-Prediction-in-Crypto-Stocks
This repository contains the code and resources for the master's thesis "The Comparison of The Performance of Open-Source LLMs In the Prediction of Price Movements of Cryptocurrencies and Stocks"  This project aims to compare the performance of various open-source Large Language Models (LLMs) in predicting the price movements of highly volatile cryptocurrencies and relatively stable stocks.
# Project Overview
The project investigates the potential of open-source LLMs (e.g., GPT-2, FinBERT, and LLaMA) in predicting price movements, focusing on their adaptability to sentiment-driven and volatility-sensitive markets like cryptocurrencies and stocks.

## Objective: Determine which open-source LLM provides the best performance for price prediction in cryptocurrencies and stocks.
## Scope: 
-Fine-tuning LLMs for financial time-series forecasting.
-Evaluating hybrid approaches, such as combining LSTM with FinBERT and GPT-2.
-Comparative analysis of the models' performance using metrics like MSE, RMSE, and Directional Accuracy (DA).
# Features
## Data Sources:

### Cryptocurrency Data: Collected using the ccxt library from major exchanges (e.g., Kraken).
### Stock Data: Collected using yfinance for stocks like Apple (AAPL) and Tesla (TSLA).
## LLMs Used:

- GPT-2, FinBERT, and other transformer-based models (e.g., LLaMA) from the Hugging Face library.
- LSTM as a baseline model and integrated with hybrid approaches (e.g., LSTM + FinBERT).
  
## Data Preprocessing:

- Data normalization and scaling for both cryptocurrencies and stocks.
- Feature engineering, including moving averages and volatility calculations.
  
## Modeling:

- Fine-tuning various LLMs for time series prediction by converting OHLCV (Open, High, Low, Close, Volume) data into sequences suitable for LLMs.
- Combined sentiment data (via FinBERT) with historical price data to enhance predictions.
- Evaluating performance across different time periods and assets.
  
## Evaluation:

- Comparative analysis of the LLMs’ performances on stocks and cryptocurrencies.
- Metrics: Mean Squared Error (MSE), training loss, and visualization of predicted vs actual prices.

# Project Structure
## Data Collection:
- ccxt is used to fetch cryptocurrency data (e.g., Bitcoin and Ethereum).
- yfinance is used to collect stock data (e.g., Apple, Tesla).
## Preprocessing:
- Data cleaning, normalization using MinMaxScaler, and missing value handling via forward/backward filling.
## LLM Fine-Tuning:
- LLMs from Hugging Face are fine-tuned on the OHLCV data, treating historical price data as sequences for prediction.
## Evaluation:
- Each LLM is evaluated based on its ability to predict future prices with MSE as the primary evaluation metric.

# Requirements
- Python 3.x
- TensorFlow or PyTorch (depending on the model)
- Hugging Face transformers
- ccxt (for cryptocurrency data)
- yfinance (for stock data)
- pandas, numpy, and scikit-learn (for preprocessing)

# Results
The models were evaluated on both cryptocurrency and stock datasets. Key findings include:

- Hybrid models (e.g., LSTM + FinBERT) demonstrated superior performance, particularly in cryptocurrency markets where sentiment plays a critical role.
- LLaMA achieved competitive accuracy in both volatile and stable markets due to its advanced transformer architecture.

# Acknowledgments
I would like to express my sincere gratitude to Prof. Dr. Visieu Lac and Prof. Schneider for their invaluable guidance, support, and feedback throughout this research. This work would not have been possible without their insights and encouragement.









