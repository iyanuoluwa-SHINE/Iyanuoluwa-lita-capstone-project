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

### Data Preparation (Excel)
In Excel, we performed essential data cleaning steps:

**Removing Duplicates :** Removing Duplicates  to prevent double-counting revenue.

**Handling Missing :** Hnandling Missing  Values in crucial fields such as Order ID and Revenue.


**Date Formatting :** Formatting Date  to standardize date fields.
**Revenue Calculation :**   Validation using formulas to cross-check **Quantity * Unit Price** against recorded revenue.

### **Data Storage and Querying (Using SQL)**

The cleaned data was then imported into SQL tables to facilitate complex querying, aggregation, and analysis, improving data handling efficiency. Key queries included:

1. **Regional Sales Aggregation**: By grouping the sales data by region, we were able to identify high-revenue areas and explore product preferences in each.
2. 
3. **Customer Revenue by Subscription Type**: Using SQL, customers were segmented by subscription type, highlighting which customer groups contributed the most revenue.
4. 
5. **Sales Trends Analysis**: SQL queries were utilized to track monthly and quarterly revenue trends, identifying periods of high and low sales to understand seasonal impacts.

### **Data Analysis and Visualization (Using Power BI)**

Data Visualization (Power BI)
**Sales by Region –** Bar charts display revenue across regions, spotlighting top-performing areas.

**Subscription Breakdown –** Pie and bar charts visualize revenue by subscription type, helping identify high-value segments.

**Sales Trend Analysis –** Line graphs illustrate monthly revenue trends, highlighting peak and off-peak periods.

Limitations
Data Completeness: Some records had missing data, which may impact accuracy.
Historical Data: Limited historical data may restrict trend analysis depth.

Recommendations
Automated Data Integration: Implement SQL-to-Power BI automation for real-time updates.
Enhanced Customer Segmentation: Further break down subscription types for deeper insights.
Predictive Analytics: Apply predictive modeling for future revenue trends.

Conclusion
The Lita Capstone Project successfully provided valuable insights into revenue drivers, customer preferences, and regional performance. By combining Excel, SQL, and Power BI, the project offers a strong foundation for data-driven decision-making and strategic growth.


