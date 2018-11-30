Zillow Data Scraper
===========================

Zillow home listings scraper, using Selenium.
WARNING: Use this code at your own risk, scraping is against Zillow's TOC.
Code takes input for query to Zillow and then outputs results to CSV

Requirements:
- Python 3.5.
- Scraping is done with Selenium v3.0.2, which can be downloaded here:
  http://www.seleniumhq.org/download/
- The selenium package requires a webdriver program. This code was written
  using Chromedriver v2.25, which can be downloaded here:
  https://sites.google.com/a/chromium.org/chromedriver/downloads

Example of the output dataframe:
------------------------

```
df.head(n=6)
```

```
                address     city state    zip    price  sqft bedrooms  \
0         4251 Drake St  Houston    TX  77005   895000  3501        4   
1  6534 Westchester Ave  Houston    TX  77005  1325000  2720        3   
2     2635 Centenary St  Houston    TX  77005  1449000  4114        5   
3     2336 Robinhood St  Houston    TX  77005  1295000  3652        3   
4     3135 Bissonnet St  Houston    TX  77005   359000  1692        2   
5         3824 Byron St  Houston    TX  77005  1100000  3161        3   

  bathrooms days_on_zillow           sale_type  \
0       4.0              4      House For Sale   
1       3.0              8      House For Sale   
2       5.0             NA      House For Sale   
3       4.0             33      House For Sale   
4       2.5             37  Townhouse For Sale   
5       4.0             43      House For Sale   

                                                 url  
0  http://www.zillow.com/homes/for_sale/27825953_...  
1  http://www.zillow.com/homes/for_sale/27792196_...  
2  http://www.zillow.com/homes/for_sale/27812119_...  
3  http://www.zillow.com/homes/for_sale/27836800_...  
4  http://www.zillow.com/homes/for_sale/27834549_...  
5  http://www.zillow.com/homes/for_sale/27823372_...
```
