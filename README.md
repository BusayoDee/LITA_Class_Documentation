# LITA_ClASS_DOCUMENTATION

### PROJECT TITLE:RETAIL STORE AND MARKET SALES REPORT

###  Overview
This project collects and analyzes sales data from various regions, markets and stores. The goal is to provide insights into the revenue, units sold and transaction categories over different periods. The analysis focuses on understanding revenue trends and sales performance across regions and calculating key metrics such as total revenue by region to determine which region is the top and least performer in terms of revenue.

### Data Collected
The dataset includes the following key columns:
1.	Region: The geographical area where the store is located
2.	Market: The specific market segment or category within a region
3.	Store: The individual store from which the sales data is collected
4.	Fiscal Period: e fiscal quarter period to which the trade date belongs
5.	Model: The Product model being sold
6.	Line of Business: The business category under which the sales falls
7.	Day Category: The kind of day the transaction was made e.g workday or public holiday
8.	Transaction Category: The category of items being sold
9.	Unit sold: The count of the quantity of item being sold
10.	Revenue: The total monetary value generated from each sale

### Project Objectives
This Project was designed to address the following analysis goals
1.	Revenue by Region: Determine the total revenue generated in each region 
2.	Region by units sold: Analyze the number of units sold across different regions
3.	Average Revenue by Region: Calculate the average revenue in each region to assess performance

### Key Metrics
1.	Revenue: Sum of the revenue grouped by region
2.	Unit sold: Sum of units sold grouped by region
3.	Average Revenue: Calculated as total revenue/total units sold for each region
   
### How to Use the Data
1.	Revenue by Region: Group the data by region and sum the revenue column. This shows an overview of how much revenue each region is generating
2.	Units sold by region: Group the data by region and sum the units sold to identify which regions are selling the most product and which is the least.
3.	Average Revenue by Region: To get the Average revenue in a region, use the formula


  ### Formula Used

  ```
Average Revenue = Total Revenue / Unit Sold

  ```
### Tools and Method Used
#### Data Analysis
The Data was analysed using microsoft Excel with the use of pivot tables  to organize and filter the data for easy interpretation, Bar charts and Column charts were created in excel to visually represents key insights


  ### Data Visualisation and Inference
### 1. REVENUE BY REGION
 

  ![bar chart](https://github.com/user-attachments/assets/11895f9b-32fc-4f97-9601-54d92035aee7)



It can be infered that North East Region generated the highest Revenue closely followed by South West while North Central appears to be lagging behind in terms of revenue generation, it  therefore suggest that there is a challenge being faced in that region and the market condition and competitive analysis needs to be done to determine why North Central stores and Markets are not doing good numbers compared to other region
  
![regionby sum of unit sold](https://github.com/user-attachments/assets/dbf6e4df-946d-423e-90e4-27ab5b5393da)





![average revenue by region](https://github.com/user-attachments/assets/4a3495fd-e96f-489a-acc7-d7d4662f77a0)






### PROJECT TITLE: SALES REPORT FOR INTERNATIONAL BREWRIES
  
###  OVERVIEW
This project collects and analyzes sales data from various sales rep of the store intenationally. The goal is to provide insights into the revenue, units sold and transaction categories over different periods. The analysis focuses on understanding revenue trends and sales performance across regions and calculating key metrics such as total revenue by region to determine which region is the top and least performer in terms of revenue.

### DATA COLLECTED
The dataset includes the following key columns:
1.	Sales ID: The transaction ID of the Sale
2.	Sales Rep: The Name of the Sales Representative for each sale
3.	Unit Price: Cost per unit of each brand
4.	Brands: The name of the particular Product being sold
5.	Quantity: The count of the sale made by each sales rep pe
6.	Cost: The cost of each product
7.	Profit: The Profit made on each sale after cost deduction
8.	Country: The particular country that the sale was made
9.	Region: The region where the sale was made
10.	Month: The month the sale was made
11.	Year: The year the sale was made

### PROJECT OBJECTIVES
This Project was designed to address the following analysis goals
1.	Profit by Region: Determine the total profit generated in each region 
2.	Region by Quantity sold: Analyze the number of quantity sold across different regions
3.	Top Performing Sales Rep: Analyze the performance of sales rep across all the regions in terms of income generation
4.	Bestselling Product per region: Analyze the bestselling brand based on profit made from each

### KEY METRICS 
1.	Profit: Sum of the Profits grouped by region
2.	Quantity: Sum of units sold grouped by region
3.	Top performing Sales_Rep
4.	Bestselling Product Brand

### HOW TO USE THE DATA
1.	Revenue by Region: Group the data by region and sum the Profit column. This shows an overview of how much revenue in terms of Profit each region is generating
2.	Units sold by region: Group the data by region and sum the quanity sold to identify which regions are selling the most product and which is the least.
3.	Top performing Sales_Rep: Group the data by the Sale_Rep and the Sum of Profit Column, this gives an insights into the total Profit being generated by each Sales_Rep

### FORMULA/ QUERY USED
1.	PROFIT BY REGION
```
select Region, sum(profit) as Region_Profit from InternationalBreweries
group by Region order by 2 desc
```
2.	QUANTITY SOLD PER REGION
```
select Region, sum(Quantity) as Region_Quantity from InternationalBreweries
group by Region order by 2 desc
```

3.	TOP PERFORMING SALES REP
```
select Sales_Rep, sum(profit) AS Sales_Profits from InternationalBreweries 
GROUP BY Sales_Rep order by 2 desc
```

### TOOLS AND METHODS USED
1.	Data Analysis: The data was analyzed with Microsoft excel using pivot tables to organize and filter the data for easy interpretation.
2.	SQL: SQL Query was as well used to query the database to get more insights into the data

### DATA VISUALIZATION 
Bar charts and Column charts were created in excel to visually represent the key insights.
1.	Profit by Region
   
2.	Quantity Sold Per Region

   
3.	Top Performing Sales Rep
   
4.	Total Profit by Brand
   




  
