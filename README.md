# yahoo-finance-analysis

For this project, I created a program to scrape Yahoo Finances most active stock page (https://finance.yahoo.com/most-active). Using Beautiful Soup, I automated scraped throught the 415 most active stocks. A loop collected necessary table data and saved them into a list that was then converted to a Pandas DataFrame. This data was then cleaned and analyzed for potential trends. 

First, Data was cleaned by dropping all duplicates and changing necessary datatypes. The format of various columns were changed due to them containing String characters, such as "B" or "%". Additionally, unnecessary columns were dropped due to containing null values. 

Furthermore, Data was organized into separate DataFrames based on stock characteristics.

    -- DataFrame for stocks with over a Trillion Dollars in Market Cap
    -- DataFrame for stocks between a Billion and a Trillion Dollars in Market Cap that have a positive Price/Earning Ratio
    -- DataFrame for stocks between a Billion and a Trillion Dollars in Market Cap that did not have a Price/Earning Ratio

Using Hvplot, the first two DataFrames were plotted to analyze the relation between PE Ratio and Stock Price. 

P/E Ratios help highlight the belief of a stock's growth with relation to their current value. This relation can help inform what companies might be undervalued, overvalued or properly valued. Through this table, individuals can see what stocks correlate with each price and PE ratio to help inform better financial decision making.

