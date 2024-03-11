# StockPortfolioAnalysis

## Introduction
DISCLAIMER: I am not an expert on financial topics, this is just a side-project for me to apply topics i have learned in class.
Python project, used yahoo finance api to get live and historcal stock prices dating back to 2017.

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/e5a7828a-b229-4484-9734-485188d03725)

My idea for this project stems from a mock stock portfolio that i had created in 2017 and recently re-discovered. The Yahoo finance portfolio i have consists of 6 stock Bank of America (BAC), Alphabet/Google (GOOG), Apple (AAPL), Nvidia (NVIDIA), AMD (AMD) and Tesla (AMD). 


![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/ee4ebf4d-43c1-47b8-a565-11696c1eac28)

### Method

In python we obtain stock data from yahoo finance via yfinance and compute the annualized perfomance of the 6 stock portfolio (mean returns, standard dev, covariance matrix). We then generate different portfolios by randomly creating different weights and multiplying them to obtain a plot of attainable portfolios. 

ie. For two securities:
![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/7009c76a-4041-4ef1-8a89-5dc4729b55c2)
![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/b1b26989-f392-4d90-a443-dbe5b776a058)

The x-axis of the generated plots indicates the volatility (Portfolio's standard deviation) and the y-axis is the expected return. From the plots we would be able to see something called the Efficient Frontier, which is a set of optimal portfolios that offer the highest expected return for a given level of risk (or lowest risk given a level of expected return). We see this frontier in our plots where we see a pattern of densely packed dots representing various portfolios. These portfolios form an arched line, illustrating the optimal trade-off between expected return and risk. To pick the optimal portfolio we compute Sharpes Ratio which quantifies and indicates how much excess return a portfolio generates for each unit it takes. (higher sharpe ratio = better).

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/2e39b215-a86e-42e5-94d3-a1437a8c0f85)

### Results

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/4033d379-2922-428f-85f3-536cefe5163a)

The results from the original portfolio show:


![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/1994804f-6b99-4a24-be85-8868d7eb0d38)


As we observed from the outcomes above, the Max Sharpe Ratio Portfolio allocating  70.32% of our stock in Nvidia, with the whole portfolio yielding annualized volatility of 0.43. On the other hand, the Min Volatility Portfolio suggests a lower annualized return but with reduced volatility. Although we have optimally rebalanced within the portfolio slightly, this still does not fix our over-reliance Nvidia stock.

## Diversified Portfolio 

Using different combination of stocks and now adding ETFs into the mix, we now obtain a more diversified portfolio. In this portfolio i allocated shares to TD Bank (TD.TO), Apple (AAPL), AON , and AMD. The two ETFs are Utilities Select Selector SPDR Fund (XLU) and Vanguard Total Stock Market Index Fund (VTI).

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/02d06579-e1a0-44f2-9246-99924c01d291)


![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/c4213c41-e0c3-4832-99b0-ad722dbb2a39)

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/cf1e4caa-b05b-46ea-8956-3b06d15d1ced)


The attainable portfolios in this diversified portfolio provide a better balance of stocks, achieving the Max Sharpe Ratio Portfolio with a lower 34% annualized return but also exhibiting lower volatility. The difference in volatility between the two attainable portfolios is evident when comparing the two graphs. In the undiversified portfolio, the points tend to deviate from the efficient frontier, whereas in the diversified portfolio, the attainable portfolios tend to hover around the efficient frontier.
