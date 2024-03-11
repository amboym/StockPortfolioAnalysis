# StockPortfolioAnalysis

## Introduction
DISCLAIMER: I am not an expert on financial topics, this is just a side-project for me to apply topics i have learned in class.
Python project, used yahoo finance api to get live and historcal stock prices dating back to 2017.

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/e5a7828a-b229-4484-9734-485188d03725)

My idea for this project stems from a mock stock portfolio that i had created in 2017 and recently re-discovered. The Yahoo finance portfolio i have consists of 6 stock Bank of America (BAC), Alphabet/Google (GOOG), Apple (AAPL), Nvidia (NVIDIA), AMD (AMD) and Tesla (AMD). Given the heavy reliance on the semiconductor sector for gains, Id like to implement a strategy to diversify the entire portfolio and use the Markowitz Portfolio Theory to determine the optimal stock allocation.


![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/ee4ebf4d-43c1-47b8-a565-11696c1eac28)

## Method and Results

We generated random portfolios and random weights to create a plot of attainable portfolios for n = 100,000. In Python, we compute the portfolio's standard deviation (volatility or risk) on the x-axis and expected return on the y-axis. We find the optimal solution by selecting the portfolio with the maximum Sharpe ratio or one with the minimum volatility.

From the plot, the cluster of orange dots forms an arch or curve known as the efficient frontier. It earns this name because among the attainable portfolios, it represents the same level of risk with the highest target return.

![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/4033d379-2922-428f-85f3-536cefe5163a)

The results from the original portfolio show:
![image](https://github.com/amboym/StockPortfolioAnalysis/assets/162647158/1994804f-6b99-4a24-be85-8868d7eb0d38)

As we observed from the outcomes above, the Max Sharpe Ratio Portfolio allocating  70.32% of our stock in Nvidia, with the whole portfolio yielding annualized volatility of 0.43. On the other hand, the Min Volatility Portfolio suggests a lower annualized return but with reduced volatility. Although we have optimally rebalanced within the portfolio slightly, this still does not fix our over-reliance Nvidia stock.

Opting for the minimum volatility portfolio offers less risk. But i think that we are still heavily reliant on tech stocks and the US markets.

## Diversified Portfolio 


