# 🍕 Pizza Sales SQL Analytics Project

## 📌 Project Overview
Analysis of a year's worth of sales data for a fictional pizza place. The goal was to answer critical business questions regarding sales trends, inventory management, and customer preferences using advanced SQL techniques.

**Tools Used:** MySQL, MySQL Workbench

**Dataset:** The dataset is provided as a ZIP file containing four CSV files:
- orders.csv
- order_details.csv
- pizzas.csv
- pizza_types.csv

## 📂 Database Schema
I designed a relational database with the following normalized tables:
- **`orders`**: Order ID, date, and time.
- **`order_details`**: Granular item-level data (pizza_id, quantity) linking orders to pizzas.
- **`pizzas`**: Product catalog with size and price information.
- **`pizza_types`**: Descriptive details (name, category, ingredients).

## 🔍 Key Business Insights
- **Peak Times:** The busiest hours are **12 PM - 1 PM** and **5 PM - 7 PM**.
- **Top Category:** **Classic** pizzas are the most popular by volume, while **Chicken** pizzas drive higher average ticket size.
- **Best Sellers:** The **Thai Chicken Pizza** is the highest revenue-generating item.
- **Sales Trends:** Fridays and Saturdays contribute **~35%** of weekly total revenue.

## 💻 Key SQL Techniques Demonstrated
- **Data Aggregation:** `GROUP BY`, `SUM`, `COUNT` to summarize sales.
- **Complex Joins:** Inner and Left Joins to combine data across 4 tables.
- **Window Functions:** `RANK()` to identify top performers and `SUM() OVER()` for cumulative totals.
- **CTEs (Common Table Expressions):** Used for breaking down complex ranking logic.
- **Time-Series Analysis:** Extracted insights by hour, day, and month.
