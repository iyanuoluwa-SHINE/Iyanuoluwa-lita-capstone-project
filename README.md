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
```SQL







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


**POWER BI**
SALES DATA
![Screenshot (89)](https://github.com/user-attachments/assets/7b8c9a20-6207-4be1-9350-ed5d88958a9a)

CONSUMER DATA

![Screenshot (88)](https://github.com/user-attachments/assets/acaca69c-8fe2-497b-a8cb-ae001a03a52d)












































### **Limitations**
**Data Completeness:** Some records had missing data, which may impact accuracy.

**Historical Data:** Limited historical data may restrict trend analysis depth.

### Recommendations 
**Automated Data Integration:** Implement SQL-to-Power BI automation for real-time updates.

**Enhanced Customer Segmentation:** Further break down subscription types for deeper insights.

**Predictive Analytics:** Apply predictive modeling for future revenue trends.

### Conclusion 
The Lita Capstone Project successfully provided valuable insights into revenue drivers, customer preferences, and regional performance. By combining Excel, SQL, and Power BI, the project offers a strong foundation for data-driven decision-making and strategic growth.


