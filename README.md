# finance
## This was the last task in Harvard_CS50 before the final project.
'finance' is a Flask web application which simulates managing portfolios of stocks by quering [IEX](https://iextrading.com/developer/)-api for stocks' prices.
### Usage
This app allows users to register for an account (login and logout have already worked). When logged in users may see their current portfolio. It is an HTML table with every row summarizing number of shares of separate holding along with its current price and total cost of shares beeing hold. New users will see empty table. Logged in users can quote stocks (i.e. look up a stocks' current price), 'buy' and 'sell' stocks (quoted since when registered each user provided Total 10000 points which are not real money and stocks beeing bought or sold are virtual). Any way quoted prices remain actual. Logged in users can also see transactions history (HTML table with detailed information of every 'buy' and every 'sell').
### Specification
Explaination what each of the files contains and does.
#### register.html
Following 'Register' link in the top right corner of the 'Log in' page redirects user to the 'Register' page. A new user inputs 'Username', 'Password' and 'Password confirmation'. If 'Password confirmation' and 'Password' fields are not epty and coincide, and if 'Username' is not empty and is unique for the site the new User will be logged in and redirected to the main (index) page. Otherwise the new User will recieve warning.
#### index.html
This file represents portfolio table. It is an HTML table. Every row holds data for single stock in the columns: 'Symbol', 'Name', 'Price', 'Price bought' and summarizes number of shares hold in the column 'Shares' as well as total cost of the stock in the column 'Total'. Column 'Price' represents current price of the stock on the moment the page was updated or the last transaction with this stock commited. Column 'Price bought' shows price of the stock the last time when it was bought. Every row also holds 'buy' and 'sell' buttons as well as input field named 'trn_shares' to specify number of shares of current symbol beeing 'sold' or additionally 'bought'. If user has enough cash-points when buying or enough shares hold when selling than transaction will be commited, current stock price will be updated again right before commiting transaction and will be shown in the 'Price' column as well as total cost of shares left for current stock in the 'Total' column. Total cost of the whole portfolio and total cash left in the bottom of the table will be updated as well. Otherwise, if something went wrong user will recieve warning.
#### quote.html
This page allows a user to query stock's current price. If symbol input was correct, after 'Quote' button clicked a user will recieve a response beneath the 'Quote' button with the name of the company and stock's current price and button 'Buy' embedded. The 'Buy' button redirects a user to the 'Buy' page with current symbol as default for 'Symbol' input. When quoting empty or incorrect symbol a user will recieve warning.
#### buy.html
#### sell.html
#### history.html
