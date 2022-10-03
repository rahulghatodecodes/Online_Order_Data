# Walmart Data

Order ID	Order Date	Ship Date	Customer Name	Country	City	State	Postal Code	Region	Category	Sub-Category	Product Name	Sales	Quantity	Discount	Profit


## Objective
- Data Transformation
- Data Modelling
- Data Visualization

## Programming Language & Tools:
- Python:
  Data Manupulation, using Pandas library.
  Data Computation, using Numpy library.
  Data Visualtion using Matplotlib & Seaborn libraries
- Jupyter Notebook
- Microsoft SQL Server Management Studio (SSMS)
- Microsoft Power BI

## Tasks: 
- Using dropna function, getting rid of rows where all the column values are null.
- Using replace function, fixed multiple instances of "country" column.
- In data imputation, replaced the null values of "Sales" column with mean
- Using Order by keyword, extracted the products giving us the highest profit.


select customer_name, product_name, state, profit, returned
from Walmart join Return_Order
on order_id = orders

