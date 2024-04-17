# Buy-and-Hold vs. RSI Trading Strategy Comparison

## Introduction
This repository contains a Python script that compares the performance of a buy-and-hold strategy against a Relative Strength Index (RSI) based trading strategy using historical stock data from Yahoo Finance. The script analyzes the performance of these two strategies on Coca-Cola (KO) stock from 2016 to 2021, providing insights into their returns and risks.

## Usage

### 1. Importing Packages
- **numpy** (as np): For numerical operations.
- **pandas** (as pd): For data manipulation and analysis.
- **yfinance** (as yf): For downloading historical stock data from Yahoo Finance.
- **matplotlib.pyplot** (as plt): For visualization.

### 2. Downloading Stock Data
- The code downloads historical stock data for the specified stock symbol (`'KO'` for Coca-Cola) from January 1, 2016, to March 21, 2021, using the `yf.download()` function from the Yahoo Finance API.

### 3. Specifying Strategy Parameters
- `rsi_period`: Specifies the lookback period for calculating the RSI indicator (in this case, 14 days).
- `rsi_oversold`: Specifies the threshold for the RSI indicator to indicate oversold conditions (typically set to 30).
- `rsi_overbought`: Specifies the threshold for the RSI indicator to indicate overbought conditions (typically set to 70).
- `fee`: Specifies the transaction fee for buying and selling stocks (set to 0.05% or 0.0005).

### 4. Coding Technical Analysis Signals
- Calculates the daily returns, Upward movement, Downward movement, Relative Strength (RS), and RSI (Relative Strength Index) based on the provided formulae.

### 5. Simulating Trading Strategies
- Computes the returns and risks for both the Buy-and-Hold (BnH) strategy and the RSI-based strategy.
- The BnH strategy simply holds the stock throughout the entire period.
- The RSI-based strategy buys when the RSI falls below the oversold threshold and sells when the RSI exceeds the overbought threshold.

### 6. Visualizing the Results
- Prints the return and risk of both strategies.
- Plots the cumulative returns of both strategies over time.
