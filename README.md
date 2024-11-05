# LITA_CLASS_DOCUMENTATION

## PROJECT TITLE:RETAIL STORE AND MARKET SALES REPORT

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







## PROJECT TITLE: SALES REPORT FOR INTERNATIONAL BREWERIES

  
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
10.	Month: The month the sale was made
11.	Year: The year the sale was made



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
```SQL
select Region, sum(profit) as Region_Profit from InternationalBreweries
group by Region order by 2 desc
```

2.	QUANTITY SOLD PER REGION
   
```SQL
select Region, sum(Quantity) as Region_Quantity from InternationalBreweries
group by Region order by 2 desc
```

3.	TOP PERFORMING SALES REP
   
```SQL
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

   
3.	Top Performing Sales Rep

   ![intern 3](https://github.com/user-attachments/assets/4c9f740d-31ad-4241-935d-17a62836f54f)

   
4.	Total Profit by Brand
   
![Intern 4](https://github.com/user-attachments/assets/e0780b55-0b6c-4e1e-8c5c-b687e8209eef)

### INFERENCE AND CONCLUSION

1.	It can be inferred that SOUTHSOUTH Region makes the most sales and generates the  most Profit and closely followed by WEST Region

2.	It can be inferred that NORTHWEST makes the least sales and generates the  least Profit for the company, this suggest a cahallenge in sales performance, this needs to be addressed by the company
   
3.	It can be deduced that JONES is the Top perfoming Sales_Rep in terms of Sales and Profit generation while HOWARD is the least Performing Sales_Rep
	
4.	It can be concluded that CASTLE LITE tops the chart as the best selling Product Brand  with a profit of 34,606,980 as well as BUDWEISSER  31,568,500 this is a wide profit margin compared to the other product brands



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

![hr1](https://github.com/user-attachments/assets/8b05f584-8b91-48f6-a813-f63339dd0141)


### Inference

 1. It can be deduced that a total number of 237 Employee have left the company with the attrition rate to be 16%
 2. The company currently has a total of 1233 Employee
 3. The department with the highest count of attrition is R&D while the department with the least attrition count is HR
 4. The Average age of Employee in the company is 37
 5. Based on the attrition count by gender, we have more males leaving the company than females
 6. It can be infered that based on the current Employee the current age range with the highest staff is age band (35-44)years and next to that is (25-34)years 

#### Filtered chart by Educational Field
#### Human Resource

![hr2](https://github.com/user-attachments/assets/72d73f43-560d-4e33-8b6c-99d9a7ee1a25)


-	It Can be inferred that Employee in HUMAN RESOURCE field are currently 20 in the company and 7 have left with attrition rate of 26%


#### Life Science

![hr3](https://github.com/user-attachments/assets/7c0c00eb-583c-4d2b-82d4-2930c7c1ce7c)



-	It can be inferred that the total number of Employees in R&D Field are currently 517 and 89 have left the company with attrition rate of 15%


#### Marketing

![hr 4](https://github.com/user-attachments/assets/f37eec8a-d38a-4941-8426-0ba8b010c409)


-	It can be inferred that the total number of Employees in MARKETING field are currently 124 and 35 have left the company with attrition rate of 22%


#### Medical 

![hr5](https://github.com/user-attachments/assets/4b526d59-3c43-4424-8465-7f46ae0ec9df)


-	It can be inferred that the total number of Employees in MEDICAL field are currently 401 as 63 have left the company with attrition rate of 14%


#### Techical


![hr6](https://github.com/user-attachments/assets/ece9c666-9466-43ea-a835-937b0ee9b4a0)


-	It can be inferred that the total number of Employees in TECHNICAL field are currently 100 and 32 have left the company with attrition ratee of 24%


### Conclusion and Recommendations
- R&D Department has the highest count of Attrition,this could be due to a lot of factors which could be salary related,  too much workload, job satisfaction or, work life balance, the company needs to take a look at this factors so as to reduce the attrition rate in R&D Department.
  
- The Company can put together a survey that all Employees can highlight whatever issues being faced on the job so it can be addressed so the company will not keep loosing good hands to probably competitors.

- The company has more Employees in their most productive years in the Company.
  






## PROJECT 4: CAPSTONE STORE SALES REPORT

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
   
```SQL
Select Product,sum(Quantity) As SALES FROM CapstoneSalesData
group by Product order by 2 desc
```
4.	Total Revenue per Product:
```SQL
select product,sum(Revenue) AS TotalRevenue from CapstoneSalesData 
group by product order by 2 desc
```

5.	Monthly Sales Totals for the current Year (2024):
```SQL
Select Datename(Month, OrderDate) AS Sales_Month, Sum(Quantity) AS Monthly_Sales2024
from CapstoneSalesData where year(OrderDate) = '2024'group by Datename(Month, OrderDate) order by Monthly_Sales2024 desc
```

6.	Top 5 Customer by total purchase amount:
```SQL
select top 5 Customer_Id, sum(Revenue) As Total_Purchase from [dbo].[CapstoneSalesData] 
group by Customer_Id order by Total_Purchase desc
```



### Data Visualization
Pivot tables, charts (bar, doughnuts,pie) were used as well as a powerbi dashboard created to visualize key insights

1. Total Sales by Product
   
![sales1](https://github.com/user-attachments/assets/7afe6518-5d25-415b-be6f-0d3535f79e7f)


2. Total Sales by Region

![sales 2](https://github.com/user-attachments/assets/5112fa2c-df81-442b-a188-6f625f4f5aaf)


3. Total Revenue by Product

![sales 3](https://github.com/user-attachments/assets/753e0819-a513-48b9-adb0-2b6c2e86efbb)

4. Monthly Sales Totals for 2024
   

![s monthly sales totals](https://github.com/user-attachments/assets/3c51fd21-f257-4c89-b1bf-a54ef729d61f)

5. Top 5 Customers by Purchase amount
   
![s top five cust](https://github.com/user-attachments/assets/9cf2564f-130f-4d10-aec8-10363f34d2dd)



![Capssalesrep](https://github.com/user-attachments/assets/1463fb5a-cf24-4c94-89f6-bf1d4a8f7d59)




### Inference and Conclusion

- It can be deduced that the highest selling products by total Sales Value is HAT closely followed by SHOES while SHIRT and GLOVES have equal number of quantity sold or sales value. We can say that a great percentage of the Stores customers are lovers of Hat or Shoes
  
- The Product that generates the most revenue is SHOE and the Product with the least revenue generated is SOCKS. It can be concluded that  is the Top performing Product for Capstone Store is SHOES

- In terms of Quantity of Product sold per Region, SOUTH REGION tops the chart, followed by EAST. This suggest there could be a challenge in sales perfomance in WEST and NORTH as the regions are not doing good numbers in terms of sales quantity
  
-  It can be inferred that SOUTH Region brings in the highest percentage in terms of Revenue generation followed by EAST region with NORTH and WEST as well lagging in revenue generation
   
-  The top five customers by the total purchase amount is CUS1488, CUS1375, CUS1023, CUS1059 AND CUS1367.


### Recommendations
- Capstone  store can stock more of Products like Shoes and Hats as they are highly in demand.
   
- The Store needs to analyze market conditions and competition in North and West Regions, then  put strategies in place  to boost performance in those region, this is crucial for improved sales and Revenue across the regions
  
-  The Top customers of Capstone Store should be identified as  Premium customers and can be given a discount on their purchases for a given period through a loyalty card , this will serve as an incentive for customer retention




## PROJECT TITLE:CAPSTONE CUSTOMER SUBSCRIPTION REPORT

### Overview: 
This Project analyzes the customer data for a subscription service to identify segments and trends. The goal is to understand customer behavior, track subscription types, and identify key trends in cancellations and renewals.

### Data Collected
The dataset includes the following key columns:

1.	CustomerID
2.	CustomerName
3.	Region
4.	SubscriptionType
5.	SubscriptionStart
6.	SubscriptionEnd
7.	Cancelled
8.	Revenue

### Key Metrics
1.	SubscriptionDuration: This Column was created and calculated as SubscriptionEnd Minus SubscriptionStart(SubscriptionEnd- Subscription start)
2.	Revenue: Sum of Total Revenue generated 
3.	Average Subscription Duration: Calculated as Subscription type grouped by SubscriptionDuration summarized by Average 


### Project Objectives
This Project was designed to address the following analysis goals:
1.	Average Subscription Duration: Determine the average Subscription duration
2.	Most Popular Subscription Type: Evaluate the most popular subscription types by the number of customers
3.	Total number of customers in each region: Retrieve the total number of customers from each Region
4.	Customers who canceled their subscription duration within 6 months: Determine customers who canceled their subscription within 6 months
5.	Customers with subscription longer than 12 months: Analyse Customers with subscription longer than 12 months
6.	Total Revenue by Subscription type: Calculates total revenue by Subscription type
7.	Top 3 Region by subscription cancellations: Determine the top 3 Region by subscription cancellations
8.	Total number of active and canceled subscriptions

### Tools and Methods Used
1.	Data Analysis: The data was analyzed with Microsoft excel using pivot tables to organize and filter the data for easy interpretation.
2.	SQL: SQL Query was as well used to query the database to get more insights into the data
3.	PowerBi: To create a dashboard for visualization of the of key customer segment.

### How to Use the Data
1.	Average Subscription Duration:  Group data  by subscriptiontype  and subscription duration ( SubscriptionEnd -SubscriptionStart) and determine the Average, this points out the average subscription duration.

2.	Most Popular Subscription Type: Group data by SubscriptionType   by the  total number of customers

3.	Total number of customers in each region: Group data by the Region and the total number of customers, this indicates the total number of customers in each region

4.	Customers who canceled their subscription duration within 6 months: With SQL Query, determine customers who canceled their subscription within 6 months, this identifies customers with canceled subscription within 6 months.


5.	Customers with subscription longer than 12 months: With SQL Query, Analyse Customers with subscription duration longer than 12 months, this identifies customers with subscription above 12 months

6.	Total Revenue by Subscription type:  Group data by Revenue and Subscription type, this calculates total revenue generated by each Subscription type.

7.	Top 3 Region by subscription cancellations: Use SQL Query to Determine the top 3 Region by subscription cancellations.

8.	Total number of active and canceled subscriptions: Use SQL Query to determine the Total number of Active and Canceled Subscription.


### Formular / Query Used

1.	Average Subscription Duration:
```   
=Total Subscription Duration / Total Number of Subscription Types
```

2.	Most Popular Subscription Type: 

Group data by subscription type by CustomerID and summarize values by Count, this shows the total number of subscribers for each subscription type.
```SQL
select top 1 SubscriptionType, count(customerID) AS Total_Customers
from CapstoneCustomerData group by SubscriptionType order by Total_Customers desc
```

3.	Total number of customers in each region: 
```SQL
select region, count(CustomerID) AS CustomerPerRegion from CapstoneCustomerData
group by Region
```
4.	Customers who canceled their subscription duration within 6 months:
``` SQL 
select CustomerID from CapstoneCustomerData where datediff (month, SubscriptionStart, SubscriptionEnd)<= 6
```

5.	Customers with subscription longer than 12 months:
``` SQL 
SELECT CustomerID, CustomerName, SubscriptionStart, SubscriptionEnd, 
datediff(month, SubscriptionStart, SubscriptionEnd)
AS Suscription_Duration From [dbo].[CapstoneCustomerData] 
where Canceled = '0' AND SubscriptionEnd IS NOT NULL AND Datediff(month, SubscriptionStart, SubscriptionEnd)> 12
```
6.	Total Revenue by Subscription type: 
```SQL
Select  SubscriptionType AS Subscription_Type, Sum(Revenue) AS Total_Revenue 
from CapstoneCustomerData group by SubscriptionType
```

7.	Top 3 Region by subscription cancellations: 
```SQL
select top 3 Region, count(canceled) As Canceled_Subscriptions from [dbo].[CapstoneCustomerData] where canceled = 'True'
group by Region
```

8.	Total number of active and canceled subscription:
 ``` SQL 
Select count(CASE WHEN Canceled = 0 THEN CustomerID END) AS Active_Subscriptions,
count(CASE WHEN Canceled = 1 THEN CustomerID END) AS Cancelled_Subscriptions from CapstoneCustomerData
```


### Data Visualizations

Pivot tables, charts (bar, doughnuts,pie) were used as well as a powerbi dashboard created to visualize key insights
1. Average Subscription Duration
   
![avesub](https://github.com/user-attachments/assets/1eba3b3c-2cc9-46a8-9d72-538c54cf251d)


2.Most  popular Subscription type

![most popular](https://github.com/user-attachments/assets/928102d7-b1b7-4919-92de-1655d6174361)


3.Total Number of customers in each region

![su custregion](https://github.com/user-attachments/assets/27f3ad87-256c-46fa-acce-3dfc8208f9a3)


4. Total Revenue by Subscription Type
   
![revbysub](https://github.com/user-attachments/assets/ec769122-ad44-43d7-b330-b3a1fd0055f6)


6. Number of Active and Canceled Subscriptions

![su actican](https://github.com/user-attachments/assets/57621a85-573f-42a2-9a7e-0bb21a6cd14b)

![capscust](https://github.com/user-attachments/assets/c94ca24d-3988-406d-82c9-1a8abbf3f7c2)


### Filtered Chat by SubscriptionType

#### BASIC

![Sub1](https://github.com/user-attachments/assets/8a5a99ce-dc87-415d-96d2-a8a7f4584d98)


- The total count of BASIC Subscribers is 37500 and it has more ACTIVE Subscribers than canceled



#### PREMIUM

![sub2](https://github.com/user-attachments/assets/fe34938e-70b5-4605-b602-fb6648f138ad)


-	The total count of PREMIUM Subscribers is 18750 and PREMIUM has 60% Canceled Subsciription.

-	Premium generates all the revenue for the South Region



##### STANDARD

![sub3](https://github.com/user-attachments/assets/4e4a363d-9b23-4f2d-9fa6-c9cf74f89866)


-	The total count of PREMIUM Subscribers is 18750 and STANDARD has 40% Active Subsciription
-	Standard  subscription generates all the revenue in the West


### Inference and Conclusion
- BASIC is the most popular subscription type and its generates more Revenue, followed by PREMIUM amd lastly STANDARD 
  
- The Average Subscription Duration is 365days which is 12 months and there is no Customer or Subscriber whose subscriptions exceed 12months
  
- No Customer or Subscriber cancelled their Subscription within 6months  
  
- SOUTH Region generates the highest form of Revenue and NORTH Region generates the least. 


















