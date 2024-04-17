# Buy-and-Hold vs. RSI Trading Strategy Comparison for Coca-Cola (KO) stock from 2016 to 2021

### Step 1: Clone the Repository
1. Open your command line interface (CLI) or terminal.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository:
   ```
   git clone <repository_url>
   ```
   Replace `<repository_url>` with the URL of the GitHub repository.

### Step 2: Download Python
1. Visit the official Python website at [python.org](https://www.python.org/downloads/).
2. Download the latest version of Python for your operating system.
3. Follow the installation instructions provided on the website.

### Step 3: Set up Jupyter Notebook
1. Open your command line interface (CLI) or terminal.
2. Install Jupyter Notebook by running the following command:
   ```
   pip install jupyterlab
   ```
3. Once installed, start Jupyter Notebook by running the following command:
   ```
   jupyter notebook
   ```
4. This will open a new tab in your web browser with the Jupyter Notebook interface.

### Step 4: Install Required Dependencies and Libraries
1. Navigate to the directory where you cloned the repository.
2. Open a new terminal or command prompt in that directory.
3. Run the following command to install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
   This command will install all the necessary packages listed in the `requirements.txt` file.

### Step 5: Run the Code on Jupyter Notebook
1. In the Jupyter Notebook interface, navigate to the directory where you cloned the repository.
2. Click on the Python script file (e.g., `buy_and_hold_vs_rsi.ipynb`) to open it.
3. Follow the instructions provided within the notebook to execute the code cells.
4. To run the code cells, click on each cell and press Shift + Enter or click the "Run" button in the toolbar.
5. The code will download the historical stock data, perform analysis, and visualize the results within the notebook.

# Introduction
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
<img width="592" alt="Screenshot 2024-04-17 at 18 29 32" src="https://github.com/yllvar/buy-and-hold-vs-rsi/assets/73235926/a1331b55-52b0-41d0-839e-6ff30990a73e">

