# AdventreWorks-Sales Analysis
## Dataset Introduction
<a href="https://github.com/sahilm20/AdventreWorks-Sales-Analysis/blob/main/AdventureWorks%2BRaw%2BData.zip">View dataset</a>
### Sales Data:
The data contains 56,000+ instances (rows) and 8 columns. 

Here's an overview of the columns:
- OrderDate: The date when the order was placed.
- StockDate: The date when the stock was available.
- OrderNumber: Unique identifier for each order.
- ProductKey: Identifier for the product.
- CustomerKey: Identifier for the customer.
- TerritoryKey: Identifier for the sales territory.
- OrderLineItem: Line item number within the order.
- OrderQuantity: Quantity of the product ordered.
### Customer Lookup:
The second data contains 18,154 instances (rows) and 13 columns. 

Here's an overview of the columns:

- CustomerKey: Unique identifier for each customer.
- Prefix: Title (e.g., Mr., Mrs., Ms.).
- FirstName: Customer's first name.
- LastName: Customer's last name.
- BirthDate: Customer's date of birth.
- MaritalStatus: Marital status (M for Married, S for Single).
- Gender: Customer's gender.
- EmailAddress: Customer's email address.
- Annual Income: Customer's annual income.
- Total Children: Total number of children.
- EducationLevel: Level of education.
- Occupation: Customer's occupation.
- Homeowner: Indicates if the customer is a homeowner (Y or N).

### Calendar lookup: It contains 912 instances (rows) and 1 column. 
Here's the column detail:
- Date: A date value ranging from January 1, 2020, onward.

Apart from this, the dataset contains 5 more tables named as Product lookup, Product category lookup, Product subcategory lookup, Territory lookup, Returns Data.
## Data Modelling
- Customer Lookup -> Sales Data | (Customer key)
- Territory Lookup -> Sales Data | (Territory key)
- Territory Lookup -> Returns Data | (Territory key)
- Calendar Lookup -> Sales Data | (Date->Orderdate, stock date)
- Calendar Lookup -> Returns Data | (Date->returnsdate)
- Product Lookup -> Sales Data | (Product key)
- Product Lookup -> Returns Data | (Product key)
- Territory Lookup -> Sales Data | (Territory key)
- Product Lookup -> Product subcategory lookup | (ProductSubcategory key)
- Product Lookup -> Product category lookup | (ProductCategory key)

![advent BI data model](https://github.com/user-attachments/assets/61d92976-5002-44b4-9772-8f66b7ea1cca)
## Introduction to dashboard
#### <a href="https://www.linkedin.com/posts/sahilmishra-tf2003_powerbi-dashboard-datavisualization-activity-7284205867627921408-63sY?utm_source=share&utm_medium=member_desktop">View dashboard</a>

### 1) Exec dashboard
#### Card visual for:
- Revenue
- Profit
- Total orders 
- Return Rate
#### Line chart showing weekly revenue trends
#### KPI Cards for:
- Monthly Revenue
- Monthly orders
- Monthly returns
#### Bar chart showing category-wise total orders
#### A matrix table for order, return and revenue of the top 10 products

![image](https://github.com/user-attachments/assets/2080b042-7760-4939-ab28-0808b3786b38)

![image](https://github.com/user-attachments/assets/f43051db-e195-46f0-bb69-59639d4a9197)

### 2) Map page
#### Map visual to analyse the number of orders by region/Country.
- Includes slicers to filter data 
#### Card visual for total customers and average revenue per customer.
#### Pie chart for total orders by income level and total orders by occupation
#### Line chart showing weekly trends of customers

![image](https://github.com/user-attachments/assets/92a12118-3e16-4a12-bae1-c6984deedeb1)

### 3) Product detail page:
#### Gauge visual to compare monthly orders, revenue and profit with the month's target(if not achieved - turns Red)
#### Area charts for profit and returns trends of that single product
- both charts have a date hierarchy as a data field, therefore we can drill through Month<->Quarter<->year.
![image](https://github.com/user-attachments/assets/7e29fe6c-66cc-4fc7-b4e4-ae458b4cade5)






