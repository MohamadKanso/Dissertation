
# Bitcoin Trading Bot with LSTM, Linear Regression, and Indicators

This repository contains the source code for a Bitcoin trading bot developed using Python. The bot utilizes various machine learning techniques, including Long Short-Term Memory (LSTM) networks and Linear Regression, to predict Bitcoin price movements and automate trading on the Binance platform.

## Project Overview

The project aims to develop an automated trading bot that evaluates live and historical market data to place trades in real time, leveraging the Binance API for data acquisition and trade execution. The bot was trained and tested on technical indicators such as Moving Averages, RSI, and MACD, using a detailed Exploratory Data Analysis (EDA) to inform feature selection.

## Libraries Used

This project uses the following libraries:

<p align="center">
  <img src="https://pandas.pydata.org/static/img/pandas_white.svg" alt="Pandas" height="40">
  <img src="https://numpy.org/doc/stable/_static/numpylogo.svg" alt="NumPy" height="40">
  <img src="https://matplotlib.org/_static/logo2_compressed.svg" alt="Matplotlib" height="40">
  <img src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" alt="Scikit-learn" height="40">
  <img src="https://seaborn.pydata.org/_images/logo-wide-lightbg.svg" alt="Seaborn" height="40">
  <img src="https://pytorch.org/assets/images/pytorch-logo.png" alt="PyTorch" height="40">
  <img src="https://www.tensorflow.org/images/tf_logo_social.png" alt="TensorFlow" height="40">
  <img src="https://keras.io/img/logo.png" alt="Keras" height="40">
  <img src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Yahoo_Finance_Logo.png" alt="Yahoo Finance" height="40">
  <img src="https://user-images.githubusercontent.com/17782624/65192519-89980e00-daa2-11e9-882e-004d2b95a72b.png" alt="Binance API" height="40">
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6e/Joblib_logo.svg" alt="Joblib" height="40">
</p>

## Key Features

- **Data Collection and Preprocessing**: Utilizes the Binance API to fetch Bitcoin market data with 15-minute intervals, converted to a structured format for analysis.
- **Exploratory Data Analysis (EDA)**: Examines trends, volatility, correlations, and technical indicators to inform model choice and setup.
- **Model Development**:
  - **LSTM Model**: Designed to capture sequential data patterns in Bitcoin price changes.
  - **Linear Regression Model**: A simpler model for benchmarking against LSTM.
  - **Naive Baseline**: A baseline model using recent price as a predictor for comparison.
- **Backtesting**: Conducts backtesting to simulate trading scenarios using historical data.
- **Live Trading**: Integrates with Binance API to execute live trades based on model predictions.


## Performance Metrics

- **Root Mean Squared Error (RMSE)** and **Mean Absolute Error (MAE)** for predictive accuracy.
- **R-squared (R²)** for Linear Regression model fit.
- **Test Score (RMSE)** and **R-squared** for model comparison.

## File Structure

- `data/`: Stores raw and processed Bitcoin data.
- `notebooks/`: Contains Jupyter notebooks for EDA, model training, and backtesting.
- `live_trading.py`: Script for live trading using Binance API.
- `requirements.txt`: List of dependencies.

## Limitations & Future Work

- **Alternative Models**: Consider testing non-linear models such as Decision Trees, Random Forest, or CNNs, which may capture complex patterns better than linear models.
- **Risk Management**: Additional risk management techniques could help stabilize returns.


