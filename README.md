# Udacity AI for trading course

Personal repository for storing quizes and notebooks from Udacity AI for trading nano degree.

## 2. Folder description

### Lesson 2

**Stock prices**

Lesson about stocks and common terminology. `stock_data.upynb` contains example of stock data set: open, close, high and low prices.

### Lesson 3

**Market mechanics**

`resample_data.ipynb` shows how to resample time data, e.g. get close price every 3rd day or every week.

### Lesson 5

**Stock returns**

Contains a quiz asking to compute returns for each ticker and date in close.

### Lesson 6

**Momentum trading**

`dtype.ipynb` contains an example how to generate position (Long 30 share of stock when the price is above 50 dollars 
or hort 10 shares when it's below 20 dollars). `top_and_bottom_performing.ipynb` shows how to filter out stocks by their performance.

### Lesson 10

**Regression**

`test_normality.ipynb` shows how to check whatever distribution is normal using Shapiro-Wilk or Kolmogorov-Smirnov methods.
`regression.ipynb` investigates to stocks using regression. 

### Lesson 11

**Time series modeling**

Example of autoregressive moving average (ARIMA) fit on time series data is shown in `autoregression_quiz.ipynb`.

### Lesson 12

**Volatility**

`rolling_windows.ipynb`shows how to annualize volatility using rolling window method.

### Lesson 13

**Pairs trading and mean reversion**

`pairs_cadidates.ipynb` shows how to check if two stocks prices correlate in time.

### Lesson 15

**Stocks, Indices, Funds**

Shows how to calculate cumulative returns.

### Lesson 17

**Portfolio risk and return**

Shows how to calculate covariance matrix.

### Lesson 18

**Portfolio optimization**

Shows to to solve portfolio optimization problems using `cvxpy` package.

### Lesson 22

**Factors**

Introduces to open source Zipline package which is used to create pipelines for stock algorithmic trading.

### Lesson 24

**Risk factor models**

Notebooks provides answers to quizzes how to calculate covariance of assets, factor model returns on assets or portfolio, and variance of portfolio or historical data.

### Lesson 26

**Risk factor models with PCA**

Introduces to principle component analysis (PCA) usage on factors. 

### Lesson 27

**Alpha factors**

Shows how to smooth alpha factors, calculate factor quantiles and ranks, how to calculate sharpie ration, transfer coefficient, z-scores.

### Lesson 28

**Alpha factor research methods**

Provide examples,how to implement alpha factors into trading strategy using overnight returns or regression against time as alpha factors. 

### Project 1

**Trading with Momentum Project**

A very simple trading strategy is implemented on quotemedia historical stock data `project_1_starter.ipynb`. 
The main idea is to buy top 10 best performing and short top 10 worst performing stocks. 

### Project 2

**Breakout strategy**

In `project_2_starter.ipynb` breakout strategy is implemented, which buys or shorts stocks, which prices beat 5, 10 or 20 day period historical prices. Signal filtering is also implemented to reduce number of trades. 

### Project 3

**Smart Beta and portfolio optimization**

In this project, betas (risk factors) are calculated for stock portfolio based on paid dividends amd returns. Then portfolio optimization is done to minimize variations. Finally, this portfolio is compared to benchmark index.

### Project 4

**Alpha research and factor modeling**

In this project, statistical risk model is built using PCA. Then model is expanded using 5 alpha factors:

* `Momentum 1 Year Factor` the hypothesis "Higher past 12-month (252 days) returns are proportional to future return.",
* `Mean Reversion 5 Day Sector Neutral Factor`, the hypothesis "Short-term outperformers(underperformers) compared to their sector will revert." 
* `Mean Reversion 5 Day Sector Neutral Smoothed Factor` just smoothed factor,
* `Overnight Sentiment Factor`, hypothesis "overnight returns reveals information about investors sentiments",
* `Overnight Sentiment Smoothed Factor` just smoothed factor.

These factors are then combined into Zipline pipeline. Model is then evaluated using factor-weighted returns, quantile analysis, sharpe ratio, and turnover analysis. Finally, the stock portfolio is optimized using multiple optimization formulations.

## Requirements

All requirements are available on `requirements.txt` file.