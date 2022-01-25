# StockScreener
This is a project in all in one solution to provide information for investing in real time

![stockscreenr](https://user-images.githubusercontent.com/62877852/150923593-0ea59dac-7cad-45d1-89d9-3c0a86fe0d07.gif)




<h2>Stocks Input Scraping</h2>

List of the companies through SP500, Russell, and self inputted
<li>Getting SP500 stocks info from wikipedia</li>
<li>Getting russell stocks info
</li>
<li>Adding own list of stocks info</li>
<h2>Yahoo Stocks Price Scraping with Pandas DataReader</h2>
<li>Find the shareprice by year and the following metrics:</li>
<h2>Balance Sheet and Income Statement Extractions with Beautiful Soup</h2>
<li>EPS</li>
<li>ROE</li>
<li>ROA</li>
<li>Long term debt</li>
<li>Total Income</li>
<li>Debt to Equity</li>
<li>Interest Coverage Ratio</li>

![s pwiki table](https://user-images.githubusercontent.com/62877852/150923211-fdcecd26-a837-4688-b6a8-25754fded9d7.png)

## Warning Signs List based on value investing logic
* Given list of the companies, find out the feasibility to invest
    * Been in market minimal 10 years
    * Have the track records (EPS per year)
    * Have efficiency (ROE > 15%) -- Net income / shareholder equity
    * Determine manipulation (ROA > 7%) -- Net income / Total Asset
    * Have small long term debt (Long term debt <5* total income)
    * Low Debt to Equity
    * Ability to pay interest: (Interest Coverage Ratio >3) -- EBIT / Interest expenses

## Decision Machine based on Marginal Price From Stocks EPS
* Decision making from each company in terms of return rate given the value investing methodology
    * Find EPS Annual Compounded Growth Rate
    * Estimate EPS 10 years from now
    * Estimate stock price 10 years from now (Stock Price EPS * Average PE)
    * Determine target by price today based on returns(discount rate 15%/20%)
    * Add margin of safety (Safety net 15%)
    * Buy if market price is lower than the marginal price
	* Sell if market price is higher than the marginal price


