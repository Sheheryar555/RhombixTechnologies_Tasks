# RhombixTechnologies_Tasks
Data Analysis Internship Tasks - Rhombix Technologies
# Task 1.1: Data Collection & Cleaning

## Objective
Collect a dataset and clean it using Python and Pandas.

## Dataset
Titanic Dataset

## Tools Used
- Google Colab
- Python
- Pandas
- NumPy

## Cleaning Performed
- Loaded dataset
- Checked data types
- Removed duplicate rows
- Handled missing values
- Converted data types
- Saved cleaned dataset

## Files
- Task1_Data_Cleaning.ipynb
- cleaned_titanic.csv
# Task 1.2: Exploratory Data Analysis (EDA)

## Objective
Perform Exploratory Data Analysis (EDA) on the cleaned Titanic dataset.

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Analysis Performed
- Summary Statistics
- Correlation Analysis
- Heatmap
- Histograms
- Count Plots
- Box Plot
- Line Plot
- Pair Plot
- Outlier Detection

## Key Insights
- Most passengers belonged to Class 3.
- Male passengers outnumbered female passengers.
- Fare contained several outliers.
- Passenger age was concentrated between 20 and 40 years.
- Survival varied by gender and passenger class.

# Task 2.1:SQL Querying and Analysis on E-Commerce Data

## Task Overview
This task involved downloading a real-world e-commerce dataset from Kaggle, loading it into a Microsoft SQL Server 2025 database, and writing SQL queries to extract meaningful business insights — top-selling products, revenue by country, monthly revenue trends, and top customers by spend.

## Dataset
- **Source:** Kaggle — E-Commerce Dataset
- **Format:** CSV, imported into SQL Server via the Import Flat File Wizard
- **Rows:** 500,000+ transaction line items
- **Columns:** `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

## Tools Used
- Microsoft SQL Server 2025
- SQL Server Management Studio (SSMS)
- T-SQL

## Key SQL Concepts Practiced
- `SELECT` and `WHERE` — filtering transaction records
- Calculated columns — deriving revenue as `Quantity * UnitPrice`
- `GROUP BY` — aggregating sales by product, country, and month
- `ORDER BY` — ranking results to surface top performers
- `JOIN` — linking a derived `Countries` reference table back to the main transactions table
- `COUNT(DISTINCT ...)` — counting unique orders and customers within aggregates

## Insights Extracted
- **Top-selling products** by total revenue and units sold
- **Revenue by country**, identifying the highest-grossing markets
- **Monthly revenue trend**, identifying the highest and lowest revenue months
- **Top customers by lifetime spend**

# Task 2.2: KPI Tracking & Interactive Dashboard

## Objective

Create an interactive Power BI dashboard to track important e-commerce sales KPIs and visualize business performance.

## Tools Used

- Power BI
- SQL Server
- DAX

## KPIs & Visualizations

- Total Revenue
- Total Quantity
- Total Orders
- Total Customers
- Monthly Growth %
- Monthly Revenue Trend
- Top 10 Countries by Revenue
- Top 10 Products by Revenue
- Country and Month/Year filters

## Key Insights

- United Kingdom generated the highest revenue.
- Monthly revenue varied throughout the year.
- Top products and countries were identified based on revenue.
- Interactive filters allow users to explore sales performance.

# Task 3.1: Data Integration & Feature Engineering

## Objective
Combine sales, product, and customer data using Pandas and create calculated features.

## Dataset
Superstore Sales Dataset — Kaggle

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib

## Analysis Performed
- Created Sales, Products, and Customers datasets
- Merged datasets using Pandas
- Calculated Total Revenue
- Calculated Profit Margin
- Calculated Customer Lifetime Value (CLV)
- Analyzed top customers, products, and categories

## Key Insights
- Identified top customers and products by revenue.
- Compared revenue and profit across categories.
- Analyzed profit margins and customer lifetime value.

# Task 3.2: A/B Testing & Hypothesis Testing

## Objective
Compare two marketing groups using A/B testing and statistical hypothesis testing.

## Dataset
Marketing A/B Testing Dataset — Kaggle

## Tools Used
- Python
- Google Colab
- Pandas
- NumPy
- SciPy
- Matplotlib

## Analysis Performed
- Compared Ad and PSA groups
- Calculated conversion rates
- Performed Chi-square test
- Performed T-test
- Performed ANOVA
- Visualized conversion rates

## Key Insights
- Ad group conversion rate: **2.55%**
- PSA group conversion rate: **1.78%**
- Chi-square test showed a statistically significant difference.
- Ad campaign performed better in terms of conversions.

# Task 4.1: Predictive Modeling & Machine Learning

## Objective
Build basic machine learning models to predict order delivery time from historical e-commerce data.

## Dataset
Olist Brazilian E-Commerce Dataset — Kaggle

## Tools Used
- Python
- Google Colab
- Pandas
- Scikit-learn

## Analysis Performed
- Loaded and merged orders and order items data
- Calculated delivery days (target variable)
- Removed missing values and extreme outliers
- Selected price and freight value as input features
- Split data into training and testing sets (80/20)
- Built Linear Regression, Decision Tree, and KNN models
- Evaluated models using R² score and Mean Absolute Error (MAE)

## Key Insights
- Compared the three models using R² and MAE.
- Best performing model: [model name] (R² = [value], MAE = [value] days)
- Price and freight alone give modest accuracy; more features could improve predictions.

## Files
- project1_ml.ipynb

# Task 4.2: Automation & Reporting

## Objective
Automate data cleaning, analysis, and reporting using Python, and send the report to Google Sheets.

## Dataset
Olist Brazilian E-Commerce Dataset — Kaggle

## Tools Used
- Python
- Google Colab
- Pandas
- Matplotlib
- Google Sheets API (gspread)

## Analysis Performed
- Loaded and cleaned the data (removed missing values and duplicates)
- Built a monthly revenue and order count report
- Visualized monthly revenue trend
- Sent the report automatically to Google Sheets
- Created a reusable run_report() function to update the sheet with one call

## Key Insights
- Report generation is fully automated, with no manual copy-paste.
- Monthly revenue trend is visible in both the chart and the Google Sheet.
- The script can be scheduled daily or weekly (Task Scheduler or cron).

## Files
- project2_automation.ipynb
