EQ101 Market Cap Indexes
-------------------------

### Background

Market cap weighted indexes are by far the most popular indexes in all major
equity markets.

### Problem Description

Construct a `TOP500 Index` for the US market according to the following rules:

0. the candidate universe consists of all stocks in the database (US-listed stocks)
0. the index level represents the total market capitalization of the largest 500
   stocks by market cap
0. the index is rebalanced on the close of the last business day of each month.
0. make sure the index level is not affected by corporate events (such as
   dividends, shares buybacks, M&A, de-listing, etc) that result in abrupt
   change of the stock's market cap.

### Questions

0. use daily return to calculate annualized volatility and Sharpe ratio on the
   rolling 12M basis over the past 5 years.
0. calculate the maximum draw downing of the index level for the past 5 years.
0. compare performance with the S&P 500 index (should you use the S&P 500 price
   index or the S&P 500 total return index? what is the difference? Which index
   does SPY (the ETF) track?).

### Bonus Questions

0. construct a `MID500 Index` with stocks whose market cap ranks from 501
   to 1000 within the same universe. Compare the performance.
0. compare index methodology for our `TOP500 Index`, the `S&P 500 index`, and
   the `Russell 1000 index`
0. Among all stocks in the universe, what percentage of market capitalization
   does the `TOP500 Index` grabs. 

### Data

* [End of Day US Stock Prices](https://www.quandl.com/data/EOD)
* [Core US Fundamental Data](https://www.quandl.com/data/SF1)

### Reference

* Methodology - S&P 500 Dow Jones Indices
* Russell U.S. Equity Indexes Construction & Methodology,
