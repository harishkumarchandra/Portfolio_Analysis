# Portfolio Analysis

An analysis notebook that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others.

Given the historical daily returns of several portfolios, some from the firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds.Determine which portfolio is performing the best across multiple areas: volatility, returns, risk, and Sharpe ratios.

Then use this analysis to create a custom portfolio of stocks and compare its performance to that of the other portfolios, as well as the larger market (S&P 500 Index)

### Prepare the Data

1. Use Pandas to read CSV files as a DataFrame
2. Detect and remove null values
3. Remove characters and convert data types
4. Calulate returns from closing price
5. Join DataFrame into a single DataFrame

    ![returns-dataframe.png](Images/returns-dataframe.png)

### Conduct Quantitative Analysis

Analyze the data to see if any of the portfolios outperform the stock market (i.e., the S&P 500).

#### Performance Analysis

1. Calculate and plot daily returns of all portfolios.

    ![daily-returns.png](Images/daily-returns.png)

2. Calculate and plot cumulative returns for all portfolios

    ![cumulative-returns.png](Images/cumulative-returns.png)
    
#### Risk Analysis

1. Create a box plot for each of the returns 

    ![returns-box-plot.png](Images/returns-box-plot.png)

2. Calculate the standard deviation for each portfolio

    ![standard-deviation.png](Images/standard-deviation.png)

3. Determine which portfolios are riskier than the S&P 500
    
    ![riskier.png](Images/riskier.png)

4. Calculate the Annualized Standard Deviation

    ![Annualized-Standard-Deviation.png](Images/Annualized-Standard-Deviation.png)
    
#### Rolling Statistics

1. Calculate and plot the rolling standard deviation for all portfolios using a 21-day window.

    ![rolling-standard-deviation.png](Images/rolling-standard-deviation.png)

2. Calculate and plot the correlation between each stock to determine which portfolios may mimick the S&P 500.

    ![correlation.png](Images/correlation.png)

3. Choose one portfolio, then calculate and plot the 60-day rolling beta between it and the S&P 500.
    
    ![rolling-beta.png](Images/rolling-beta.png)
    
4. An alternative method to calculate a rolling window is to take the exponentially weighted moving average

    ![exponentially-weighted-moving-average.png](Images/exponentially-weighted-moving-average.png)
    
### Sharpe Ratios

1. Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot.

    ![Sharpe-ratios.png](Images/Sharpe-ratios.png)

2. Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.
    
    The above Sharpe ratio plot shows that Algo1 with 1 outperform both 'the market'(S&P 500) and the whales
