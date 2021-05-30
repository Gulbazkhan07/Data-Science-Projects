# Interactive Dashboard for RockinRobin IceCreamery
# Description of the project
The audience of the Data visualization is the executive manager and business unit of the Rockin Robin, the famous creamery. In fact, and in the annual meeting of the managers, it’s important to summarize the financial activity of the creamery and analyze the trend, the performance of the product and other insights that could lead us to eventual improvements in the next financial planning.

So, the dashboard will mainly analyze:
*	The trend and seasonality of the profit, net margins and sales
*	The performance of the different brand’s product
*	The geographic distribution of the brand products

Presenting this data visualization will help us extract insights to direct actions:
*	Market targeting and segmentation function of the area codes;
*	Better management of the costs
*	Optimizing and maximizing of the profits per product.

# Dataset
First, we will categorize the variables function of their types:
#	Continuous variables

We dispose of 11 continuous variables related to financial and performance indicators:
* 1.	Profit:	Profit generated measured (in $,000) = Margin - Total Expenses
* 2.	Margin: Net sales revenue (in $,000) = Sales - Cost of Goods
* 3.	Sales:	Operating revenue (in $,000) earned from selling IceCream/Beverages
* 4.	COGS: Cost of Goods (in $,000) that is the direct costs attributable to the production of the goods sold by the company
* 5.	Total: Expenses Total costs in (in $,000) associated with managing and operating the business (COG not included)
* 6.	Marketing: Marketing costs (in $,000)
*  7.	Inventory: Total value of products and goods (in $,000) that are ready or for sale.
* 8.	Budget Profit:	Projected profit (in $,000)
* 9.	Budget COGS: Projected cost of goods (in $,000)
* 10. Budget Margin: Projected margin (in $,000)
* 11.	Budget Sales:	Projected sales (in $,000)

#	Categorical variables

* Market	Market region (East, West, Central, South)
* Market Size	Market size as a factor of population and demand (Major vs. Small)
* Product	
* Product ID	
* Product Type	Type of ice cream and beverages sold
* Product	: Product sub-category

# Data Analysis

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Business%20insights%20of%20RockinRobin/images/geoprahical.png'>

The Beverage are the best seller product of Rockin Robin creamery. The product is present in east, west and central US. The Cup & Cones are the best seller in the US south


<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Business%20insights%20of%20RockinRobin/images/sales.png'>

The financial indicators are following a slighlty decreasing trend with important seasonality linked the effect of months on quarters and also persons habits and preferences.


<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Business%20insights%20of%20RockinRobin/images/top3.png'>
The Ultimate Sundae is the best seller product in all US country. The Top 3 products change from state to another depending on the customer needs and geographic location

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Business%20insights%20of%20RockinRobin/images/boxplot.png'>

The Boxplot, dhow that the dessert are sunday have high variance meaning that their values fluctuates strongly depending on the day, month and seasons

<img src='https://github.com/Gulbazkhan07/Data-Science-Projects/blob/main/Business%20insights%20of%20RockinRobin/images/dashboard.png'>

The Rockin Robin dataset contains many referential data that could be used as interactive component of the dashboards:

* The State filter is an important component that would be used to make a zoom or focus on a specific US state.
* The Financial indicators are also displayed as interactive component in order to make the dashboard show the zoom based on the each chosen financial indicator.
* 	We could also add interactive components linked to the product, the product type and the area code to make the dashboard more interactive.






