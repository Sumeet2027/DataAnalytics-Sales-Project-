# 📊 SQL Data Analytics Project

> **End-to-End Sales Data Analysis using SQL Server**

Welcome to my **SQL Data Analytics Project**! 👋

This project demonstrates how I use **SQL Server to explore, analyze, and transform sales data into meaningful business insights**. The analysis focuses on sales performance, products, customers, categories, revenue, and year-over-year trends.

The project was built as a practical way to develop my **real-world Data Analyst skills**, from exploring raw data to creating analytical reports and business KPIs.

---

## 🎯 Project Objective

The main objective of this project is to answer important business questions using SQL and identify patterns in:

* 💰 Sales & Revenue
* 📦 Product Performance
* 👥 Customer Behavior
* 🏷️ Category Performance
* 📈 Sales Trends
* 📊 Business KPIs

---

## 🔄 Project Workflow

```text
                Sales Dataset
                     │
                     ▼
              Data Import
                     │
                     ▼
             Data Exploration
                     │
                     ▼
              Data Analysis
                     │
          ┌──────────┼──────────┐
          ▼          ▼          ▼
       Sales      Products   Customers
       Analysis   Analysis   Analysis
          │          │          │
          └──────────┼──────────┘
                     ▼
           Performance Analysis
                     │
                     ▼
              Business KPIs
                     │
                     ▼
            Business Insights
```

---

## 🗂️ Dataset Structure

The project uses a simple **fact and dimension table structure**.

### Fact Table

```text
dbo.fact_sales
```

Contains transactional sales information such as:

* Order number
* Order date
* Product key
* Customer key
* Sales amount
* Quantity

### Dimension Tables

```text
dbo.dim_products
dbo.dim_custome
```

These tables provide additional information about:

* Products
* Categories
* Subcategories
* Customers
* Customer details

---

## 🔍 Analysis Performed

### 1. Data Exploration

I first explored the dataset to understand its structure and identify the available:

* Tables
* Columns
* Products
* Customers
* Categories
* Orders
* Sales data

---

### 2. Sales Analysis

Analyzed overall sales performance including:

* Total revenue
* Total quantity sold
* Total orders
* Revenue by category
* Revenue by product
* Revenue trends over time

---

### 3. Product Analysis

Analyzed product performance to identify:

* Top 5 products by revenue
* Low-performing products
* Product categories
* Product sales performance
* Product revenue segments
* Average selling price

---

### 4. Customer Analysis

Analyzed customer behavior including:

* Top customers by revenue
* Total orders per customer
* Total quantity purchased
* Customer spending
* Customer recency
* Customer segments

Customers were categorized into:

```text
VIP
Regular
New
```

---

### 5. Performance Analysis

Performed year-over-year product analysis using SQL window functions.

The analysis compares:

* Current-year sales
* Previous-year sales
* Average product sales
* Year-over-year difference
* Sales increase/decrease

---

## 📊 Customer & Product Reports

The project also creates reusable SQL views for reporting.

### Customer Report

```text
dbo.report_customers
```

Includes:

* Customer information
* Age group
* Customer segment
* Total orders
* Total sales
* Total quantity
* Total products
* Recency
* Average order value
* Average monthly spend

### Product Report

```text
dbo.report_products
```

Includes:

* Product information
* Category
* Subcategory
* Product segment
* Total orders
* Total sales
* Total quantity
* Total customers
* Recency
* Average selling price
* Average order revenue
* Average monthly revenue

---

## 🧠 SQL Techniques Used

This project helped me practice and apply real-world SQL concepts such as:

```text
SELECT
WHERE
GROUP BY
ORDER BY
JOIN
LEFT JOIN
CASE
CTE
Aggregate Functions
Window Functions
LAG()
AVG() OVER()
COUNT()
SUM()
DATEDIFF()
YEAR()
ROUND()
Views
```

---

## 📈 Business Questions Answered

Some of the key questions answered through this project are:

* What is the total revenue generated?
* Which categories generate the highest revenue?
* Which products generate the highest revenue?
* Which products have the lowest sales performance?
* Who are the top customers by revenue?
* How does product performance change year over year?
* Which customers generate the most revenue?
* What is the average order value?
* What is the average monthly revenue?
* Which products are high, medium, or low performers?

---

## 🛠️ Tools & Technologies

| Tool           | Purpose                           |
| -------------- | --------------------------------- |
| **SQL Server** | Data analysis & reporting         |
| **SSMS**       | SQL development                   |
| **SQL**        | Data exploration & analysis       |
| **Git**        | Version control                   |
| **GitHub**     | Project documentation & portfolio |

---

## ▶️ How to Run the Project

### 1. Install SQL Server

Install:

* SQL Server
* SQL Server Management Studio (SSMS)

### 2. Create a Database

Create your database in SQL Server.

```sql
CREATE DATABASE DataAnalytics;
GO

USE DataAnalytics;
GO
```

### 3. Import the Dataset

Import the sales dataset into SQL Server.

Make sure these tables are available:

```text
dbo.fact_sales
dbo.dim_products
dbo.dim_custome
```

### 4. Run the SQL Scripts

Run the scripts in the following order:

```text
01_import_data.sql
02_explore_data.sql
03_sales_analysis.sql
04_customer_analysis.sql
05_product_analysis.sql
06_performance_analysis.sql
07_reports.sql
```

### 5. View the Reports

After creating the views, run:

```sql
SELECT *
FROM dbo.report_customers;
```

and:

```sql
SELECT *
FROM dbo.report_products;
```

---

## 📁 Project Structure

```text
SQL-Data-Analytics-Project/
│
├── datasets/
│   └── sales_dataset.csv
│
├── scripts/
│   ├── 01_import_data.sql
│   ├── 02_explore_data.sql
│   ├── 03_sales_analysis.sql
│   ├── 04_customer_analysis.sql
│   ├── 05_product_analysis.sql
│   ├── 06_performance_analysis.sql
│   └── 07_reports.sql
│
├── README.md
└── LICENSE
```

---

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

* Writing SQL queries for business analysis
* Exploring and understanding datasets
* Using joins to combine business data
* Creating customer and product reports
* Calculating business KPIs
* Using CTEs and window functions
* Performing year-over-year analysis
* Creating reusable SQL views
* Converting raw data into business insights

---

## 🚀 Future Improvements

I plan to extend this project by adding:

* 📊 Power BI dashboard
* 📈 Interactive business KPIs
* 🔄 Automated ETL pipeline
* 📋 Advanced customer segmentation
* 📉 More advanced sales analysis

---

## 👨‍💻 About Me

Hi, I'm **Sumeet**.

I am an aspiring **Data Analyst** who enjoys working with data and solving business problems using analytics.

### My Skills

```text
SQL
Power BI
Excel
Python
Data Analytics
Data Cleaning
Data Visualization
ETL
Data Warehousing
```

I am continuously improving my skills through **hands-on projects** and practical problem-solving.

My goal is to turn raw data into **clear, useful, and actionable business insights**.

---

## ⭐ Project

If you find this project useful, feel free to explore the repository and give it a ⭐.

**Thanks for visiting! 🚀**
