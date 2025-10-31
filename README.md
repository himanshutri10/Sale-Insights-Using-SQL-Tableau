# India-Based Hardware Company Sales Insights

*A Data Analysis Project using Tableau and SQL*

---

## Project Overview

This project focuses on analyzing sales insights for an India-based hardware company using **Tableau** and **SQL**. It aims to uncover hidden patterns in sales performance, support data-driven decision-making, and automate insights for faster business responses.

---

## About the Project

* Conducted an end-to-end data analysis project on sales performance for a hardware company in India.
* Designed and implemented **ETL pipelines using SQL** to extract, clean, and transform unstructured data into a structured format.
* Built a **star schema data model** and visualized it in Tableau to identify trends and KPIs across regions, years, and customer segments.
* Created **interactive Tableau dashboards** that highlight performance variations, profitability, and actionable business insights.


## Technologies Used

* **Excel**
* **MySQL** and **SQL Server**
* **Tableau** and **Power BI**
* **Statistics for Data Science using Python** with *dev help*


---

## Project Details

### Tableau Dashboard

[Dashboard](https://public.tableau.com/views/SalesInsights-DataAnalysisProjectusingTableauFromHimanshu/Dashboard-RevenueAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

### Problem Statements

The sales director wanted to assess company performance across various Indian states and regions to identify opportunities for discounts and optimization.

Key Questions:

1. Revenue breakdown by cities.
2. Revenue breakdown by year and month.
3. Top 5 customers by revenue and sales quantity.
4. Top 5 products by revenue.
5. Net profit and profit margin by market.

---

## Project Planning (AIMS Grid Framework)

### 1. Purpose

To unlock previously hidden sales insights, support data-driven decision-making, and reduce manual reporting time through automation.

### 2. Stakeholders

* Sales Director
* IT Team
* Customer Service Team
* Data & Analytics Team

### 3. End Result

An automated dashboard providing up-to-date sales and profit insights for faster business decisions.

### 4. Success Criteria

* Dashboards reveal current and accurate sales insights.
* Improved decision-making leading to 10% cost savings.
* 20% reduction in manual data gathering efforts.

---

## Data Analysis Approach

1. Extracted raw data using SQL queries.
2. Performed ETL (Extract, Transform, Load) for data cleaning and normalization.
3. Designed relational schema (Fact and Dimension tables).
4. Connected Tableau with SQL database for data visualization.
5. Created dashboards to visualize key metrics (revenue, profit, top products/customers, etc.).

---

## SQL Queries Used

Examples:

```sql
-- Show all customer records
SELECT * FROM customers;

-- Count total number of customers
SELECT COUNT(*) FROM customers;

-- Transactions from Chennai market (Mark001)
SELECT * FROM transactions WHERE market_code='Mark001';

-- Distinct products sold in Chennai
SELECT DISTINCT product_code FROM transactions WHERE market_code='Mark001';

-- Transactions using USD currency
SELECT * FROM transactions WHERE currency='USD';

-- Total revenue for 2020
SELECT SUM(t.sales_amount)
FROM transactions t
INNER JOIN date d ON t.order_date = d.date
WHERE d.year = 2020 AND (t.currency='INR' OR t.currency='USD');
```

## Author

**Himanshu Tripathi – Product Manager**
