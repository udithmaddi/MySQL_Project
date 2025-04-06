# 🕒 Time Series Analysis Using MySQL - Superstore Dataset

This project focuses on **time series data analysis using MySQL** with the Superstore dataset. The goal is to explore temporal trends, moving averages, and ranking mechanisms, and draw insights from historical sales data over time.

---

## 📁 Project Overview

- 🔍 Analyze temporal trends such as monthly/daily averages
- 📊 Evaluate sales performance using ranking and window functions
- ➕ Create lead/lag features to understand past and future data points
- 📈 Compute moving averages to reveal underlying patterns
- 🎯 Use SQL for data transformation, feature engineering, and insights

---

## 🗃️ Dataset Description

The dataset used is a sample from a retail Superstore, containing 20+ records across several years.

### The dataset includes:

- **Row ID** – Unique row identifier  
- **Order ID** – Unique sales transaction identifier  
- **Order Date** – Date the order was placed  
- **Ship Date** – Date the order was shipped  
- **Ship Mode** – Shipping method used  
- **Customer ID / Name** – Customer identifiers  
- **Segment** – Market segment (Consumer, Corporate, Home Office)  
- **Country / City / State / Region** – Location details  
- **Postal Code** – Delivery ZIP code  
- **Product ID / Name** – Product identifiers  
- **Category / Sub-Category** – Product classification  
- **Sales** – Revenue generated  
- **Quantity** – Number of items sold  
- **Discount** – Applied discount rate  
- **Sales Previous** – Sales of the previous record (via `LAG`)  
- **Sales Next** – Sales of the next record (via `LEAD`)  

---

## 🛠️ Key SQL Concepts Applied

1. **Creating & Inserting Data**  
   - `CREATE DATABASE`, `CREATE TABLE`, `INSERT INTO`

2. **Feature Engineering with Window Functions**  
   - `LAG()` for Previous Sales  
   - `LEAD()` for Next Sales  
   - `RANK()` for Sales Ranking  
   - `AVG() OVER(...)` for Moving Averages

3. **Aggregations and Time-based Grouping**  
   - Daily and Monthly Sales Averages

4. **Joins for Discount Analysis**  
   - Self joins on dates to analyze discount patterns over consecutive days

---

## 📌 Highlighted Queries

- **Previous and Next Sales Columns** using `LAG()` and `LEAD()`  
- **Sales Rankings** across all records  
- **Monthly & Daily Average Sales** grouped using `GROUP BY`  
- **Moving Average** over a 3-day window  
- **Discount Comparison** between consecutive days  

---

## 💻 How to Run This Project

1. Install and launch MySQL or use an online SQL editor like [DB Fiddle](https://www.db-fiddle.com/)
2. Copy the entire SQL script from `superstore_time_series.sql`
3. Execute it step-by-step to observe results and build understanding
4. Modify or add queries for deeper insights!

---

## 🧠 Learnings and Outcomes

- Proficiency in time-based SQL queries  
- Understanding of advanced SQL features like window functions  
- Real-world implementation of business sales data analysis  
- Developed ability to convert flat records into time-aware insights  

---
