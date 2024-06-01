# BlackPyScholes-Black-Scholes-Option-Pricing-Model
# Option Pricing Project

## Overview
This project focuses on implementing and analyzing financial options pricing using historical stock data and mathematical models. Specifically, we download historical adjusted close prices for Apple Inc. (AAPL), calculate the volatility of its stock using log returns, and then apply the Black-Scholes formula to compute the prices of European call and put options.

## Components

### Data Acquisition
We use `yfinance` to download historical stock data for AAPL from February 2, 2023, to February 8, 2024. The adjusted close prices are extracted from this dataset for further analysis.

### Volatility Calculation
The log returns of the stock are computed, and the standard deviation of these returns is used as the volatility measure (`sigma`).

### Option Pricing
We implement the Black-Scholes formula to calculate the prices of European call and put options. The functions `call_option_price` and `put_option_price` take the current stock price, strike price, time to expiry, risk-free rate, and volatility as inputs and return the respective option prices.


## Usage
1. **Download Historical Data:** The first step is to download the historical stock data for the given ticker symbol within the specified date range.
2. **Calculate Volatility:** Compute the log returns of the stock and determine the volatility.
3. **Price Options:** Use the `call_option_price` and `put_option_price` functions to price European call and put options, respectively, based on the current stock price, strike price, time to expiry, risk-free rate, and calculated volatility.

## Dependencies
- `yfinance`: For downloading historical stock data.
- `numpy`: For numerical operations.
- `scipy`: For statistical functions and normal distribution calculations.
- `math`: For mathematical functions.

## Conclusion
This project demonstrates a practical application of financial theories and computational techniques to price options using real stock market data. It can be extended to include more advanced option pricing models, sensitivity analysis, and portfolio optimization strategies.

