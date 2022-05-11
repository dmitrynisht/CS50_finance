# finance
## This was the last task in Harvard_CS50 before the final project.
'finance' is a Flask web application which simulates managing portfolios of stocks by quering [IEX](https://iextrading.com/developer/)-api for stocks' prices.
### Usage
This app allows users to register for an account (login and logout have already worked). When logged in users may see their current portfolio. It is an HTML table with every row summarizing number of shares of separate holding along with its current price and total cost of shares beeing hold. New users will see empty table. Logged in users can quote stocks (i.e. look up a stocks' current price), 'buy' and 'sell' stocks (quoted since when registered each user provided Total 10000 points which are not real money and stocks beeing bought or sold are virtual). Any way quoted prices remain actual. Logged in users can also see transactions history (HTML table with detailed information of every 'buy' and every 'sell').
### Specification
Explaination what each of the files contains and does.
#### index.html
This file represents portfolio table. It is an HTML table. Every row holds data for single stock and summarizes number of shares hold as well as current price and total cost. Every row also holds 'buy' and 'sell' buttons as well as input field to specify number of shares of current symbol beeing 'sold' or additionally 'bought'. If user has inough cash-points when buying or enough shares hold when selling than transaction will be commited, current stock price will be updated as well as total cost of current stock and total cost of the whole portfolio and total cash left. Otherwise, if something went wrong user will recieve warning.
"""""""""""""""""may be describe here colomns which might seem strange-named
#### register.html
put this file first
desctiption comes here
#### quote.html
#### buy.html
#### sell.html
#### history.html
