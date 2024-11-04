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






## PROJECT TITLE: SALES REPORT FOR INTERNATIONAL BREWRIES
  
###  Overview
This project collects and analyzes sales data from various sales rep of the store intenationally. The goal is to provide insights into the revenue, units sold and transaction categories over different periods. The analysis focuses on understanding revenue trends and sales performance across regions and calculating key metrics such as total revenue by region to determine which region is the top and least performer in terms of revenue.

### Data Collected
The dataset includes the following key columns:
1.	Sales ID: The transaction ID of the Sale
2.	Sales Rep: The Name of the Sales Representative for each sale
3.	Unit Price: Cost per unit of each brand
4.	Brands: The name of the particular Product being sold
5.	Quantity: The count of the sale made by each sales rep 
6.	Cost: The cost of each product
7.	Profit: The Profit made on each sale after cost deduction
8.	Country: The particular country that the sale was made
9.	Region: The region where the sale was made
10. Month: The month the sale was made
11. Year: The year the sale was made

### Project Objectives
This Project was designed to address the following analysis goals
1.	Profit by Region: Determine the total profit generated in each region 
2.	Region by Quantity sold: Analyze the number of quantity sold across different regions
3.	Top Performing Sales Rep: Analyze the performance of sales rep across all the regions in terms of income generation
4.	Bestselling Product per region: Analyze the bestselling brand based on profit made from each

### Key Metrics
1.	Profit: Sum of the Profits grouped by region
2.	Quantity: Sum of units sold grouped by region
3.	Top performing Sales_Rep
4.	Bestselling Product Brand

### How to use the Data
1.	Revenue by Region: Group the data by region and sum the Profit column. This shows an overview of how much revenue in terms of Profit each region is generating
2.	Units sold by region: Group the data by region and sum the quanity sold to identify which regions are selling the most product and which is the least.
3.	Top performing Sales_Rep: Group the data by the Sale_Rep and the Sum of Profit Column, this gives an insights into the total Profit being generated by each Sales_Rep

### Formula / Query Used
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
![intern1](https://github.com/user-attachments/assets/72906ba1-b3fd-4f26-bb7c-251b3c81eaf5)


   
2.	Quantity Sold Per Region

   ![Intern 2](https://github.com/user-attachments/assets/ed3f9496-684c-4a02-b5aa-47338219dee3)

   
4.	Top Performing Sales Rep

   ![intern 3](https://github.com/user-attachments/assets/4c9f740d-31ad-4241-935d-17a62836f54f)

   
6.	Total Profit by Brand
   
![Intern 4](https://github.com/user-attachments/assets/e0780b55-0b6c-4e1e-8c5c-b687e8209eef)

### INFERENCE AND CONCLUSION

1.	It can be inferred that SOUTHSOUTH makes the most sales and generates the  most Profit and closely followed by WEST

2.	It can be inferred that NORTHWEST makes the least sales and generates the  least Profit for the company
   
3.	It can be deduced that JONES is the Top perfoming Sales_Rep in terms of Sales and Profit generation while HOWARD is the least Performing Sales_Rep
	
4.	It can be concluded that CASTLE LITE tops the chart as the best selling Product Brand  as well as BUDWEISSER With a wide profit margin compared to the other brands


## PROJECT TILTLE: HR ATTRITION DATA ANALYSIS

### Overview
This project collects and analyzes employee data from various departments in an organization. The goal is to provide insights into the number of employees, Total number of attritions, Total Number of Current Employee, the attrition Rate, Attrition count by department The analysis focuses on understanding the attrition rate of the staff in the organization by age band and department.

### Data Collected
The dataset includes the following key columns:
1. Attrition: This contains Values YES or No, to show staff who have left the organization and those who are still there
2. Age band: This contains different age brackets
3. Educational Field: This shows the discipline of each employee
4. Employee Number: This shows the staff number of each employee
5. Gender: This indicates the sex of each employee
6. Job role: This is the current job role of each employee
7. Marital Status: The marital status of each employee
8. Age: The Age of each employee
9. Monthly Income: This indicates the monthly income
10. Work Life Balance: This shows different values indicating work life balance
11. Years At Company: This is the total number of years each employee has stayed In the company
12. Years in Current Role: This shows the number of years in current role
13. Job Level: This shows the current Job level
14. Job Satisfaction: This shows values to indicate job satisfaction metrics

### Project Objectives
This Project was designed to address the following analysis goals
1.	Attrition Count by Department: Determine the attrition count in each department
2.	Attrition Count by Educational Field: Analyze the attrition based on educational field
3	Attrition Count by Gender: Determine the attrition count based on gender
4	Attrition Rate:Determine the rate of Attrition in the company

### Key Metrics
1. Total Number of Employees: Totalof all the employees
2. Attrition Count: Total Count of Attrition
3. Attrition Rate: Rate of Attrition in the company
4. Average Age: Average Age of Employees
   
### How to Use the Data

1. Total Number of Employee: Create a Measure to sum and callout the total number of employee in the company
2. Attrition Count: Create a conditional Column for the count of Attrion YES and NO with 1 being for YES AND 0 for NO
3. Attrition Rate: This is calculated as the attrition count divideed by the total number of employee * 100
4. Average Age: Create a measure to find the average Age of employee in the organisation

### Tool Used
1. Microsoft Powerbi for Analysis and Visualization
   
### Data Visualization
Card Visuals, Bar charts, Pie charts, Doughnuts and slicers were used in the analysis and visualization of key insights





### Inference and Conclusion







## PROJECT 4: CAPSTONE SALES REPORT

### Overview
This project Analyzes the sales performance of a retail store. It explores Sales data to uncover key insights such as top-selling products, regional performance and monthly sales trends. The goal is to produce an interactive Power Bi dashboard that highlights these findings.

### Data Collected
The dataset includes the following key columns:
1.	OrderID
2.	Customer
3.	Product
4.	Region
5.	OrderDate
6.	Quantity
7.	UnitPrice

### Key Metrics
1.	Revenue: This Column was created and calculated as (Product of Quantity by Unit Price)
2.	Total Sales: Sum of Quantity of Products being sold
3.	UnitPrice: Cost of a single product 
4.	Order Date: The transaction Date
   
### Project Objectives
This Project was designed to address the following analysis goals:
1.	Total Sales by Product, Region and Month: Determine the total sales made by each product, each region and each Month.

2.	Average Sales per Products: Calculate the average sales per product

3.	Total Revenue by Region: Calculates the total revenue by region

4.	Highest Selling Product: Determine the highest selling Product by total sales value

5.	Total Revenue Per Product: Calculates the total revenue generated by each product

6.	Monthly Sales Totals for the current year: Determine the Monthly sales totals for the current year 2024

7.	Find the Top 5 Customer by total purchase amount: Determine the Purchase amount by each customer and filter to get the top 5.

8.	Percentage of total sales by Region: Calculates the Percentage of Total sales contributed by each Region
9.	
10.	Identify Products with no sales in the last quarter

### Tools and Method Used
1.	Data Analysis: The data was analyzed with Microsoft excel using pivot tables to organize and filter the data for easy interpretation.
2.	SQL: SQL Query was as well used to query the database to get more insights into the data
3.	PowerBi: To create a dashboard for visualization of the Sales Overview

### How to use the Data
1.	Total Sales by Product: Group the data by Product and Sum of the Quantity column with a Pivot table This shows an overview of how much Sales each Product is making.

2.	Total Sales by Region: Group data by Product and Sum of the Quantity Column with a pivot table. This shows how much is generated by each region

3.	Total Sales by Month: Group data by Month and Sum of the Quantity Columns with a pivot table This identifies sales generated in different months.

4.	Average Sales Per Product: Use the AVERAGEIF Function to calculate the Average Sales generated by each Product type.

5.	Total Revenue by Region: Use SUMIF Function to calculate the Total Revenue generated by each region.

6.	Highest Selling Product: Use SQL Query to determine the highest selling Product by total sales value.

7.	Total Revenue Per Product: Use SQL Query to Calculates the total revenue generated by each product

8.	Monthly Sales Totals for the current year:  Use SQL Query to determine the Monthly sales totals for the current year 2024

9.	Find the Top 5 Customer by total purchase amount: Use SQL Query to Determine the Purchase amount by each customer and filter to get the top 5.

10.	Percentage of total sales by Region: Use SQL Query to Calculate the Percentage of Total sales contributed by each Region

11.	Identify Products with no sales in the last quarter: Write an SQL Query to identify Products with No Sales in the Last Quarter.

### Formular / Query Used
1.	Average Sales Per Product:
   ```
=AVERAGEIF(C2:C50001,C2,F2:F50001)
```

2.	Total Revenue by Region:
   ```
=SUMIF(D2:D50001,D2,H2:H50001)
```

3.	Highest Selling Product:
   
```
Select Product,sum(Quantity) As SALES FROM CapstoneSalesData
group by Product order by 2 desc
```
4.	Total Revenue per Product:
```
select product,sum(Revenue) AS TotalRevenue from CapstoneSalesData 
group by product order by 2 desc
```

5.	Monthly Sales Totals for the current Year (2024):
```
Select Datename(Month, OrderDate) AS Sales_Month, Sum(Quantity) AS Monthly_Sales2024 from CapstoneSalesData
where year(OrderDate) = '2024'group by Datename(Month, OrderDate) order by Monthly_Sales2024 desc
```

6.	Top 5 Customer by total purchase amount:
```select top 5 Customer_Id, sum(Revenue) As Total_Purchase from [dbo].[CapstoneSalesData] 
group by Customer_Id order by Total_Purchase desc
```
7.	Percentage of total sales by region:


8.	Identify Products with No sales in the last Quarter:





