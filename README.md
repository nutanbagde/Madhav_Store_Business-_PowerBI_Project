
# Madhav_Store_Business-_PowerBI_Project

## Objective:
The owner of Madhav Store, an online retail business, seeks to develop a comprehensive sales analytics dashboard to monitor,
track, and analyze online sales performance across India. The goal is to gain actionable insights into sales trends, product 
performance, customer behavior, and regional demand to support data-driven decision-making and drive business growth.

## Business Context:
As Madhav Store expands its online presence across India, the owner requires a centralized, interactive dashboard to:
1.	Visualize key performance indicators (KPIs) such as total revenue, number of orders, and average order value.
2.	Identify high-performing products and underperforming categories.
3.	Analyze customer purchase behavior and geographic distribution of sales.
4.Track sales trends over time to anticipate demand and optimize inventory.
5.	Enable quick and informed business decisions based on real-time or regularly updated data.

## Analytical Goals:
1.	What is the distribution of total sales across different states in India?
2.	Who are the top 5 customers based on total purchase value?
3.	Which product categories and sub-categories have the highest total sales?
4.	During which month does the business generate the highest sales?
5.	What are the total sales amount, total profit, total quantity sold, and the average order value (AOV)?
6.	Which product category has the highest number of units sold?
   
## About dataset
The dataset used in this article is “E-commerce data” which is online store data. To analyse we have 2 tables 

### Table1:- Details.csv file 
* Order ID:- Identifies which order this line item belongs to.
* Amount:- The total sales amounts for this item or transaction line.
* Profit:- Net profit earned from selling the item (Amount - Cost).
* Quantity:- Number of units of the product purchased in this transaction.
* Category:- Broad classification of the product 
* Sub-Category:- More specific classification under the main category .
* PaymentMethod:- Method used for the transaction (e.g., UPI, Credit Card, Cash on Delivery).
    
### Table2:- Orders.csv file 
* Order ID:-  Identifies which order this line item belongs to.
* Order Date:- Date when the order was placed
* CustomerName:- Name of the customer
* State:- State in India where the order was delivered
* City:- City in India where the order was delivered

## Data Cleaning & Transformation
Because the data I need is in different formats, the next step is to clean the data to prepare for analysis. 
  
### Data Cleaning Steps
*  Remove Duplicates:
   Check for and eliminate duplicate rows in both Order and Details tables, especially based on Order ID.
*  Handle Missing Values
   Order Table: Check for missing State, City, or CustomerName.
   Details Table: Ensure no missing values in critical fields like Amount, Profit, Quantity, Category, or PaymentMethod.
   Missing values can be dropped, filled with defaults, or investigated depending on business context.
*  Correct Data Types:-
   Order Date to datetime format.
   Amount, Profit, and Quantity to numeric data types (float or int).
   Ensure Category, Sub-Category, and PaymentMethod are of string type or categorical.
*  Standardize Text Values:- Strip whitespaces, fix capitalization, and unify naming (e.g., “credit card” → “Credit Card”).
   Apply to columns like State, City, Category, Sub-Category, and PaymentMethod.
*  Check Relationships:-  nsure referential integrity: Every Order ID in Details should exist in Order.
  
    
## This is My Dashboard.
![Madhav_store_PowerBI.png]
## Analysis Result/Learnings
1. A user-friendly, visually rich dashboard built using tools like Power BI that provides the store owner with real-time visibility
into sales performance and customer behaviour across India, thereby improving operational efficiency and strategic planning.
2.	Used complex parameters to drill down in the worksheet and customization using filters and slicers.
3.	Created connections, join new tables, calculated to manipulate data, and enable user-driven parameters for visualization.
4.	Used different types of customized visualisation (bar chart, pie chart, donut chart, line chart, scatter chart,
      clustered bar chart, area chart, map, slicers etc.)



