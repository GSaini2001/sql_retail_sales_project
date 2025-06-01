
# 🛍️ Retail Sales Analysis SQL Project

## 📌 Project Overview

**Project Title**: Retail Sales Analysis Using SQL  
**Level**: Beginner to Intermediate  
**Database Name**: `retail_sales`

This project demonstrates foundational SQL skills used by data analysts to explore and analyze retail transaction data. It includes database setup, data cleaning, exploratory data analysis, and answers to real business questions using SQL queries. The project is ideal for practicing SQL logic and gaining insights from structured data.

---

## 🎯 Objectives

1. **Set up the retail sales database** with a structured schema.
2. **Clean the data** by identifying and removing null or missing records.
3. **Perform exploratory data analysis (EDA)** to understand patterns.
4. **Answer business questions** with focused SQL queries.

---

## 🗃️ Project Structure

### 1. Database Setup

- **Database Name**: `retail_sales`
- **Table**: `retail_sales`
- **Fields**:
  - `transactions_id`, `sale_date`, `sale_time`, `customer_id`, `gender`, `age`, `category`, `quantity`, `price_per_unit`, `cogs`, `total_sale`

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
# 🛍️ Retail Sales Analysis SQL Project

## 📌 Project Overview

**Project Title**: Retail Sales Analysis Using SQL  
**Level**: Beginner to Intermediate  
**Database Name**: `retail_sales`

This project demonstrates foundational SQL skills used by data analysts to explore and analyze retail transaction data. It includes database setup, data cleaning, exploratory data analysis, and answers to real business questions using SQL queries. The project is ideal for practicing SQL logic and gaining insights from structured data.

---

## 🎯 Objectives

1. **Set up the retail sales database** with a structured schema.
2. **Clean the data** by identifying and removing null or missing records.
3. **Perform exploratory data analysis (EDA)** to understand patterns.
4. **Answer business questions** with focused SQL queries.

---

## 🗃️ Project Structure

### 1. Database Setup

- **Database Name**: `retail_sales`
- **Table**: `retail_sales`
- **Fields**:
  - `transactions_id`, `sale_date`, `sale_time`, `customer_id`, `gender`, `age`, `category`, `quantity`, `price_per_unit`, `cogs`, `total_sale`

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
# 🛍️ Retail Sales Analysis SQL Project

## 📌 Project Overview

**Project Title**: Retail Sales Analysis Using SQL  
**Level**: Beginner to Intermediate  
**Database Name**: `retail_sales`

This project demonstrates foundational SQL skills used by data analysts to explore and analyze retail transaction data. It includes database setup, data cleaning, exploratory data analysis, and answers to real business questions using SQL queries. The project is ideal for practicing SQL logic and gaining insights from structured data.

---

## 🎯 Objectives

1. **Set up the retail sales database** with a structured schema.
2. **Clean the data** by identifying and removing null or missing records.
3. **Perform exploratory data analysis (EDA)** to understand patterns.
4. **Answer business questions** with focused SQL queries.

---

## 🗃️ Project Structure

### 1. Database Setup

- **Database Name**: `retail_sales`
- **Table**: `retail_sales`
- **Fields**:
  - `transactions_id`, `sale_date`, `sale_time`, `customer_id`, `gender`, `age`, `category`, `quantity`, `price_per_unit`, `cogs`, `total_sale`

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
2. Data Exploration & Cleaning
Performed essential checks and removed incomplete records.
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

3. Business Questions Answered
This project addresses the following key business queries:

Daily sales on 2022-11-05

Clothing sales with quantity ≥ 4 in November 2022

Total sales by category

Average customer age for 'Beauty' products

Transactions with sales > 1000

Sales count by gender and category

Top-performing months by average sale

Top 5 customers by spend

Unique customer count per category

Order count by shift (Morning, Afternoon, Evening)

Each query is written and explained in the file.
🔧 Tools Used
SQL (likely MySQL or PostgreSQL)

Any SQL execution environment (DB Browser, MySQL Workbench, SQLite, etc.)

Git & GitHub
📊 Key Findings
Sales are highest in specific categories like Clothing and Beauty.

Multiple transactions exceed 1000 in value — indicating high-value purchases.

Peak sales happen in particular shifts and months.

The top 5 customers contribute significantly to overall revenue.
🚀 How to Use
Clone the repo or download the .sql file.

Run the script in your SQL environment.

Observe results and modify queries to explore further.

🙋‍♀️ About Me
I'm Gurleen, an aspiring Data Analyst with hands-on experience in SQL, Excel, and Python. This project is part of my analytics portfolio to demonstrate my SQL capabilities and business-thinking mindset.

📫 Contact: gurleensaini564@gmail.com


