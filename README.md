# Iyanuoluwa-lita-capstone-project

# Project Overview
The Lita Capstone Project is a data-driven initiative focused on analyzing sales performance and customer data to identify revenue trends, customer preferences, and high-performing regions. Using Excel for data cleaning, SQL for querying and aggregations, and Power BI for visualizations, this project provides actionable insights that guide business strategy.


### **Data Sources**

The primary data sources for this project are the *Sales* and *Customer* datasets from the *Lita Capstone Project* file. These datasets contain detailed records essential for analyzing revenue, product preferences, and customer subscription behavior.

1. **Sales Data**: Contains transaction-level details such as order ID, customer ID, product type, region, order date, quantity sold, unit price, and calculated revenue.
2. **Customer Data**: Includes customer information, regional affiliation, subscription type, start and end dates of subscriptions, and revenue attributed to each customer.


### *Tools and Methodology*
**Excel**: Data cleaning and preprocessing

**SQL**: Data storage, querying, and aggregation

**Power BI**: Visualization and dashboard creation

### Data Preparation (Excel) [Download Here](https://microsoft-excel.en.softonic.com/)

In Excel, we performed essential data cleaning steps:

**Removing Duplicates :** Removing Duplicates  to prevent double-counting revenue.

**Handling Missing :** Hnandling Missing  Values in crucial fields such as Order ID and Revenue.

**Date Formatting :** Formatting Date  to standardize date fields.

**Revenue Calculation :**   Validation using formulas to cross-check **Quantity * Unit Price** against recorded revenue.

### **Data Storage and Querying (Using SQL)**[Download Here](https://www.microsoft.com/en-us/evalcenter/download-sql-server-2022)

The cleaned data was then imported into SQL tables to facilitate complex querying, aggregation, and analysis, improving data handling efficiency. Key queries included:

1. **Regional Sales Aggregation**: By grouping the sales data by region, we were able to identify high-revenue areas and explore product preferences in each.

2. **Customer Revenue by Subscription Type**: Using SQL, customers were segmented by subscription type, highlighting which customer groups contributed the most revenue.
 
3. **Sales Trends Analysis**: SQL queries were utilized to track monthly and quarterly revenue trends, identifying periods of high and low sales to understand seasonal impacts.

### Data Analysis and Visualization (Using Power BI)[Download Here](https://www.microsoft.com/en-us/power-platform/products/power-bi)


**Sales by Region –** Bar charts display revenue across regions, spotlighting top-performing areas.

**Subscription Breakdown –** Pie and bar charts visualize revenue by subscription type, helping identify high-value segments.

**Sales Trend Analysis –** Line graphs illustrate monthly revenue trends, highlighting peak and off-peak periods.

### Exploratory data analysis

 EDA involved the exploring of the data to answer some questions  about the data such as;

**-What Is The Total Revenue** 

**-Average Revenue**

**-Average Subsription**

### Data analysis
This is where we incclude some basic lines of code or queries;

EXCEL
```EXCEL
I. TOTAL REVENUE{NORTH}=SUMIF(D:D,"north",H:H)

II. HIGHEST PRODUCT SOLD{SHOES]=MAX(C:C,H:H)

III.LEAST PRODUCT SOLD {SOCKS}=MIN(C:C,H:H)
```
SQL
```SQ


SALES DATA 
I.the Number of Sales Transactions in Each Region

SELECT Region, COUNT(*) AS Number_of_Transactions
FROM sales_data
GROUP BY Region;

II. TOTAL SALE PRODUCT

SELECT Product, SUM(sale_of_product) AS Total_Revenue
FROM sales_data
GROUP BY Product;


III.
--------Top 5 Customers by Total Purchase Amount----

SELECT Customer_id, SUM(sale_of_product) AS Total_Purchase_Amount
FROM sales_data
GROUP BY Customer_id
ORDER BY Total_Purchase_Amount DESC

CONSUMER DATA

I.Total Number of Customers from Each Region

SELECT Region, COUNT(CustomerID) AS TotalCustomers
FROM [dbo].[Customer_Subscriptions]
GROUP BY region;

II. Most Popular Subscription Type by the Number of Customers

SELECT SubscriptionType, COUNT(CustomerID) AS NumberOfCustomers
FROM [dbo].[Customer_Subscriptions]
GROUP BY SubscriptionType
ORDER BY NumberOfCustomers DESC


III. Find the Top 3 Regions by Subscription Cancellations

SELECT Region, COUNT(CustomerID) AS Cancellations
FROM [dbo].[Customer_Subscriptions]
WHERE Canceled = 1
GROUP BY Region
ORDER BY Cancellations DESC




```

POWER BI
```POWER BI
I.Average Order-id = AVERAGE(SalesData[Customer Id])

II.AVERAGE UNIT PRICE = AVERAGE(SalesData[UnitPrice])

III.Total Revenue = SUM('CustomerData (2)'[Revenue])
```

### **DATA VISUALIZATION**

**EXCEL** SALES DATA 

Region	Sum of revenue
East	485925
North	387000
South	927820
West	300345
Grand Total	2101090
	
	
![image](https://github.com/user-attachments/assets/38ad2323-78e7-4254-9c00-eeb309a3c164)



















![image](https://github.com/user-attachments/assets/f64a1015-79bf-4dab-9dd1-9c71b801671c)



	Product	Sum of revenue
	Shirt	485600
	Shoes	613380
	Hat	316195
	Socks	180785
	Jacket	208230
	Gloves	296900
	Grand Total	2101090

 
		
![image](https://github.com/user-attachments/assets/587729b9-d4e3-4d83-8ce4-5edb080cca19)


								
![image](https://github.com/user-attachments/assets/d0d2038a-1e8f-4715-953c-38114770b1a2)



CONSUUMER DATA
	
SubscriptionType	Sum of Revenue
Basic	33776735
Premium	16899064
Standard	16864376
Grand Total	67540175


![image](https://github.com/user-attachments/assets/f92c0d33-ac93-45c8-ae4d-be1850644ab6)

								
								
								
								
								
								
								
								
								
								
								
								
								
								
								
								
								
![image](https://github.com/user-attachments/assets/0301521d-d4d3-42e9-b185-5fe3f5e33b72)

	
Region	Sum of revenue
East	485925
North	387000
South	927820
West	300345
Grand Total	2101090

	
![image](https://github.com/user-attachments/assets/feb35a30-59d4-46d4-abbc-38daca8f2f65)

















![image](https://github.com/user-attachments/assets/9f1a75d7-858d-4c58-ae57-59325995fd9f)



**sql**


sales data 
the Number of Sales Transactions in Each Region

![Screenshot (95)](https://github.com/user-attachments/assets/0709c18e-e9df-4e6d-a2d7-8730f1ff3115)


 Calculate Total Revenue per Product
 
![Screenshot (93)](https://github.com/user-attachments/assets/40bbaef8-3b94-44eb-bf0e-a271f3b6665c)

Top 5 Customers by Total Purchase Amount

![Screenshot (91)](https://github.com/user-attachments/assets/2e5dab2c-4a6d-4736-b3c2-50f113db0abd)



CONSMER DATA

Total Number of Customers from Each Region

![Screenshot (100)](https://github.com/user-attachments/assets/9d95b33e-f682-43d9-8bc6-955a20c11e2d)


Most Popular Subscription Type by the Number of Customers

![Screenshot (101)](https://github.com/user-attachments/assets/a0580979-a5a4-4057-b1e0-ed1a6374f307)


Find the Top 3 Regions by Subscription Cancellations

![Screenshot (104)](https://github.com/user-attachments/assets/e63728e4-8e2d-40e0-84ff-ebf4bc9038c4)













**POWER BI**

**Dashboard Overview**

Our project features a Power BI dashboard that provides in-depth insights into sales and consumer data. Below is an overview of each section, highlighting key metrics and visualizations that drive actionable insights.

**SALES DATA**
**Key Metrics**

**Total Order Date Count:** 449M – Represents the total count of orders by date, showing demand volume over time.

**Average Revenue:** 0.212K – Reflects the mean revenue per transaction, which helps assess overall profitability.

**Average Unit Price:** 29 – Provides insight into pricing strategies and product valuation.

**Total Revenue:** 2M – The cumulative revenue across products and regions.

**Total Order ID Count:** 9921 – Indicates the total orders, which aids in understanding customer volume.


![Screenshot (89)](https://github.com/user-attachments/assets/7b8c9a20-6207-4be1-9350-ed5d88958a9a)


**CONSUMER DATA**
**Key Metrics**

**Total Revenue:** 68M – A comprehensive sum of revenue generated across all regions and subscription types.

**Average Revenue:** 2.00K – Indicates the mean revenue generated per transaction.

**Average Subscription (Beginning):** 44.9K and (End): 45.2K – Represents subscription star and end metrics over the observed period.

![Screenshot (108)](https://github.com/user-attachments/assets/d7e589ba-dd24-4e86-a6d7-6e6825041ebe)









































### Insights
**Revenue Performance by Region:** Both dashboards show revenue contributions by region, with the South and East leading. This suggests that marketing efforts are effective in these areas, though there may be potential for growth in the North and West regions.

**Subscription Trends:** The second dashboard tracks revenue based on subscription types and dates. The high revenue from the "Basic" subscription type indicates a strong base of cost-conscious customers, while fluctuations in revenue over time may reveal seasonal or promotional effects.

**Product Sales:** The first dashboard highlights products, with Shoes generating the highest revenue. The average unit price varies widely by product, showing potential price sensitivity differences among items.

**Order Volume vs. Revenue:** The total order count is high, yet the average revenue is relatively low. This could imply a focus on lower-priced, high-turnover items or the effectiveness of budget-friendly subscription plans.

Recommendations
**Regional Marketing Strategies:** Increase engagement in North and West regions to boost their contribution to revenue. Use targeted campaigns or local partnerships in these areas, informed by existing customer behavior in high-performing regions.

**Upselling and Premium Offers:** Since "Basic" subscriptions generate the most revenue, consider upselling premium subscription features to these customers. Add value through exclusive benefits that justify the higher cost and retain users at a premium level.

**Product-Specific Promotions:** Products with lower revenue, like Socks, could benefit from targeted promotions. Bundling these items with high-performing ones or offering discounts could increase their sales.

**Subscription Retention Efforts:** With a notable portion of revenue from canceled subscriptions, develop retention strategies such as loyalty rewards, personalized communication, and subscription renewal discounts to reduce churn and maximize revenue sustainability.

**Pricing Optimization:** Experiment with strategic pricing for products, especially high-priced items like Shoes. Testing small price adjustments or implementing discount offers during peak sales periods can help maximize revenue without sacrificing profitability.

### Conclusion 
The Lita Capstone Project successfully provided valuable insights into revenue drivers, customer preferences, and regional performance. By combining Excel, SQL, and Power BI, the project offers a strong foundation for data-driven decision-making and strategic growth.💪🌟 🤝💖


