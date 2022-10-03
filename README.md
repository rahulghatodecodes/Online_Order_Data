# Walmart Data
We have a Walmart Data containing detailed information of customers who ordered some product. The dataframe contains of different variables which we will be working on are mentioned below:
- Order ID	
- Order Date	
- Ship Date	
- Customer Name	
- Country	
- City	
- State	
- Postal Code	
- Region	
- Category	
- Sub-Category	
- Product Name	
- Sales	
- Quantity	
- Discount	
- Profit

## Objective
- Data Transformation
- Data Modelling
- Data Visualization

## Programming Language & Tools:
- Python: Data Manupulation using Pandas library, Data Computation using Numpy library, Data Visualtion using Matplotlib & Seaborn libraries.
- Jupyter Notebook
- Microsoft SQL Server Management Studio (SSMS)
- Microsoft Power BI

## Tasks: 
1. Used dropna function, getting rid of rows where all the column values are null.
   - **walmart.dropna(how = 'all', inplace = True)**
2. Used replace function, fixed multiple instances of "country" column.
   - **walmart['Country'].replace({'United States': 'USA'}, inplace=True)**
   - **walmart['Country'].unique()**
3. In data imputation, replaced the null values of "Sales" column with mean.
   - **m = walmart['Sales'].mean()**
   - **walmart['Sales'].fillna(value=m, inplace=True)**
4. Used Order by keyword in SQL Server, extracted the products giving us the highest profit.
   - **select customer_name, product_name, state, profit**
   - **from Walmart**
   - **WHERE state = "California" AND customer_name = "Brosina Hoffman"**
   - **order by profit DESC limit 4**
5. Joined two tables using join in SQL Server, the second table contains the information of those order which got cancelled. We need to find the customer who cancelled the order, and the product name which got cancelled and what is the profit for that product. 
   - **select customer_name, product_name, state, profit, returned**
   - **from Walmart join Return_Order**
   - **on order_id = orders**
6. Created a interactive **dashboard** for the walmart data on Microsoft Power BI:
   <img width="955" alt="image" src="https://user-images.githubusercontent.com/98107926/193669939-6b963d66-3294-450e-8b2a-3610d6a5a727.png">
   - Used **card visual** to display total Sales, total Profit and total count of order_ID.
   - Used **area chart** to visualize Sales and Profit by Year.
   - Used **Treemap** to display Profit by category.
   - Used **Decomposition tree** to breakdown the fields further into total Sales, City, Category, Product_Name, and Customer_Name. 
   - Used **Bar Chart** to visualize total number of order by Customer_Name.
   - Used **Slicer** to filter the dashboard w.r.t particluar Customer_Name, Category, Product_Name and State.
   - Also used **QnA** feature and added to the dashboard.

