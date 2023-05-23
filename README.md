<h1 align="center"> Uncovering Market Insights: Automating E-Commerce Web Scraping for Product Research</h1>

Uncovering market insights and gaining a competitive advantage is crucial in today's dynamic business landscape. This project provides an automted web scraping solution using Selenium to extract valuable data from E-commerce sites for comprehensive market research. 

### Key Features: Expected Tangible Outcomes
+ 🔍 __Competitor Analysis__: Gained a competitive edge by analyzing rival products, pricing strategies, and customer reviews to uncover hidden opportunities.
+ 💰 __Pricing Optimization__: Utilized real-time pricing data to optimize pricing strategies, ensuring maximum profitability and market competitiveness.
+ 💡 __Product Development Insights__: Leveraged customer feedback, product specifications, and market trends to shape product development initiatives, resulting in customer-centric innovations.
+ 📈 __Market Trends and Demand Analysis__: Stayed one step ahead by monitoring market trends, customer sentiment, and demand fluctuations to drive targeted marketing campaigns and seize emerging opportunities.

#### BeautifulSoup: As of Dec 2022;
There are limitations of BeautifulSoup with different website. As frontend are built using different languages, it is often times BeautifulSoup is having a hard times in synchronizing with all of the outout during iteration. 
  + eg; for Jobstreet, the href only pointed at the company's web page instead of the job iteself. though the url shows up after inspecting the elements but it doesn't show as an output during iteration. 
  + the loop is inconsistent throughout every iteration, some iteration gives a complete href extraction of a specific url but some just return with a company'ssite only (due to /cmp instead of /rc/clk)
  
#### Selenium: As of Dec 2022;
1. Scraping and Automation with Selenium is done with MAC OS hence there are few problems encountered and solutions;
  + Problem: Path not found for chrome webdriver
  + Solution:
    1. ```brew install --cask chromedriver``` on terminal.
    2. import os
    3. change System Preference > System & Security to allow access for chromedriver.exe
    4. use ```raw``` on path info so that the slashes could be read since MAC path is different from that of Windows
    (```r/Users/apple/Downloads/chromedriver```)

2. Deprecation Error:
  + webdriver version: the chromedriver version is depends on the version of the chrome browser in your local machine. hence, please refer to the chrome version before downloading the driver. Else, once compatibility issues occur, the browser will crash after code execution. 
  + scripts to locate the element: the script/syntax of ```.find_element_by_searchfunction``` is deprecated for the newer version of Selenium. To resolve this, ```import selenium.webdriver.common.by.By``` module with the generic syntax of ```.find_element(by=By.**, value='name')```
       
#### Update as of Jan 2023: 
There a few deprecated module scripts/libraries as of 1st Jan 2023. Therefore, please refer to module documentation for more info. 

