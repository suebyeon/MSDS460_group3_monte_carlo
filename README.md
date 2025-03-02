
# Group 3 MSDS460 Monte Carlo Stock Simulation Problem 

Code, write-up, and documents for MSDS460 group A3 Monte Carlo.

## Description

In this assignment we explore the application of rules-based investing, backtesting, and Monte Carlo simulation to the financial sector,
lookin specifically at stocks in the energy sector.


### Problem Outline

Our goal was to develop an investment strategy, calculate its historical returns, and simulate its performance under varying market conditions by 
applying our strategy to Monte Carlo simulations of the underlying stocks. We developed and backtested a mean reversion investment strategy in the energy industry 
that used Relative Strength Index (RSI) and Bollinger Bands thresholds to determine buy and sell signals.
We backtested numerous variations of this investment strategy over a historical 25 year period--from 1999 to 2024--and compared them to a buy-and-hold strategy 
as well as overall market returns. 
We also conducted Monte Carlo simulations of stocks' performance during the historical period to simulate multiple market scenarios during the same period. We used
the historical returns and volatility of the underlying stocks during that period to inform the simulations.

### Results

The buy-and-hold strategy achieved a return of about ~2500% during the 25-year period, while the S&P 500 had a return of about ~500% during this same period. 
Our most successful mean reversion/RSI strategy had the following characteristics.
- Bollinger bands set at  2x above and below the standard deviation of the stock's 20-day moving average 
- RSI calculated using a 14-day period 
- Buy stocks when the price is under the lower Bollinger band and RSI is under 20
- Sell stocks when the price is over the upper Bollinger band and RSI is over 80

However, this strategy performed worse than both the buy-and-hold and market returns over the same period and only returned ~270%.

The team recommends adding more risk management strategies, such as a defined stop-loss implementation. 

## Authors

Julia O’Keeffe, Paul Yaginuma, Graham Lovell, Su Hyun Byeon, & Jacob Zott




