# 🛍️ Retail Sales Analysis SQL Project

## 📌 Project Overview

**Project Title**: Retail Sales Analysis Using SQL  

**Database Name**: `retail_sales`

This project demonstrates SQL skills commonly used by data analysts to explore and analyze sales data. It includes database setup, data cleaning, exploratory data analysis (EDA), and solving real business problems using SQL queries. The project is built using a single SQL file and is ideal for learners who want hands-on experience with practical SQL scenarios.

## 🎯 Objectives

1. Set up the retail sales database and table structure.  
2. Clean the data by identifying and removing null records.  
3. Perform exploratory data analysis to understand the dataset.  
4. Write SQL queries to answer 10 business-related questions.

## 🗃️ Project Structure

### 1. Database Setup

- Database: `retail_sales`  
- Table: `retail_sales`  
- Fields: `transactions_id`, `sale_date`, `sale_time`, `customer_id`, `gender`, `age`, `category`, `quantity`, `price_per_unit`, `cogs`, `total_sale`

```sql
CREATE TABLE retail_sales (
  transactions_id INT PRIMARY KEY,
  sale_date DATE,
  sale_time TIME,
  customer_id INT,
  gender VARCHAR(10),
  age INT,
  category VARCHAR(35),
  quantity INT,
  price_per_unit FLOAT,
  cogs FLOAT,
  total_sale FLOAT
);
```

### 2. Data Cleaning

Performed essential checks and removed incomplete records.

```sql
-- Record count
SELECT COUNT(*) FROM retail_sales;

-- Unique customers
SELECT COUNT(DISTINCT customer_id) FROM retail_sales;

-- Null check
SELECT * FROM retail_sales
WHERE 
    sale_date IS NULL OR sale_time IS NULL OR customer_id IS NULL OR 
    gender IS NULL OR age IS NULL OR category IS NULL OR 
    quantity IS NULL OR price_per_unit IS NULL OR cogs IS NULL;

-- Delete nulls
DELETE FROM retail_sales
WHERE 
    sale_date IS NULL OR sale_time IS NULL OR customer_id IS NULL OR 
    gender IS NULL OR age IS NULL OR category IS NULL OR 
    quantity IS NULL OR price_per_unit IS NULL OR cogs IS NULL;
```

## 📊 Business Questions Answered

This project answers the following key business questions:

1. Sales made on `2022-11-05`  
2. Clothing category transactions with quantity ≥ 4 in November 2022  
3. Total sales and order count by category  
4. Average age of customers in the Beauty category  
5. High-value transactions (`total_sale` > 1000)  
6. Transactions count by gender and category  
7. Best-performing months based on average sales  
8. Top 5 customers by total spend  
9. Unique customer count per category  
10. Order count by time shift (Morning, Afternoon, Evening)  

All queries are included in the `.sql` file.

## 🛠️ Tools Used

- SQL (PostgreSQL / MySQL / SQLite compatible)  
- SQL execution environment (DB Browser / MySQL Workbench / SQLite Studio / VS Code)  
- Git & GitHub

## 📄 File Included

- [`sql_retail_sales.sql`](./sql_retail_sales.sql) — contains table creation, data cleaning, and all queries.

## 📌 Key Insights

- Customers span various age groups and product categories.  
- High-value sales (> 1000) exist across several categories.  
- Clothing and Beauty were among the top-selling categories.  
- Ordering patterns vary by time of day, useful for shift-based planning.  
- Monthly trends reveal seasonal variations in customer behavior.

## 🚀 How to Use

1. Clone or download this repository.  
2. Open `sql_retail_sales.sql` in your preferred SQL editor.  
3. Run each section of the file to explore data and generate insights.  
4. Modify queries to explore more angles or dig deeper into patterns.

## 🙋‍♀️ About Me

I'm **Gurleen**, an aspiring data analyst with hands-on experience in SQL, Excel, and Python. This SQL project is part of my analytics portfolio and showcases my ability to write clear, efficient queries and solve real-world business problems using data.

📫 **Email**: gurleensaini564@gmail.com



Thank you for visiting this project! 🌟




