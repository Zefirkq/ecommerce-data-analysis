# E-Commerce Data Analysis

##  About the Project
This is my first data analysis portfolio project. The goal was to take a real-world, messy dataset, clean it, and extract basic business insights about sales, products, and customers using Python and Pandas.

##  Dataset
- **Source:** [E-Commerce Data on Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
- **Description:** Contains ~540,000 transactions from a UK-based online retail store (Dec 2010 – Dec 2011).
- **Key Columns:** `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`.

##  What I Did

### 1. Data Cleaning & Preprocessing
- Loaded the data and checked for missing values and duplicates.
- Dropped rows with missing `CustomerID` (as customer analysis is a key goal).
- Converted `InvoiceDate` to datetime format and extracted `Month` and `DayOfWeek` for easier analysis.
- Created a new `TotalPrice` column (`Quantity` * `UnitPrice`).
- Filtered out canceled orders (negative quantities) to focus on actual sales.

### 2. Exploratory Data Analysis (EDA)
- **Time Analysis:** Calculated total revenue and number of orders by month and day of the week.
- **Product Analysis:** Found the top 10 most popular products by quantity sold and by total revenue.
- **Customer Analysis:** Identified the top 10 customers by total spending and calculated the average order value.
- **Geographic Analysis:** Checked which countries generate the most revenue.

### 3. Data Visualization
Created clear and simple charts using Seaborn to visualize:
- Monthly revenue trends.
- Top selling products (bar chart).
- Sales distribution by country.

##  Key Findings
1. **Best Month:** The highest revenue was generated in November, likely due to holiday shopping.
2. **Top Product:** The most frequently purchased item was POPCORN HOLDER.
3. **Customer Base:** The majority of transactions come from the United Kingdom, which is expected for a UK-based store.
4. **Average Order:** The average customer spends approximately £534 per transaction.

## Technologies Used
- **Python** 
- **Pandas** 
- **Matplotlib & Seaborn** 
- **Jupyter Notebook** 

##  How to Run This Project
1. Download **e-com.ipynb** and **data**(from repository or Kaggle) OR clone repository
2. Install required libraries(check **requirements.txt**)
3. open and run **e-com.ipynb** notebook