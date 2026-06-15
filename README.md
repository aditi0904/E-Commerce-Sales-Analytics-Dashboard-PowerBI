# E-Commerce Sales Analytics Dashboard | Power BI

## Project Overview

This project presents an interactive Power BI dashboard built to analyze sales performance of an e-commerce business. The dashboard combines customer, product, and order data to provide insights into revenue, product performance, regional sales, cancellations, and sales trends.

The goal is to help business stakeholders make data-driven decisions by identifying top-performing products, profitable categories, high-revenue regions, and revenue losses caused by order cancellations.

---

## Business Problem

E-commerce businesses generate thousands of transactions daily, making it difficult to manually track sales performance and customer behavior.

Management needed answers to key business questions:

* Which products generate the highest revenue?
* Which categories perform best?
* Which states contribute the most sales?
* How much revenue is lost due to cancelled orders?
* How is revenue changing over time?

This dashboard was built to provide a single source of truth for monitoring business performance.

---

## Dataset Information

### Customers Dataset

Records: 462

Columns:

* CustomerID
* First Name
* Last Name
* Phone
* City
* State
* Phone Brand
* Operating System

Purpose:
Customer demographics and regional analysis.

---

### Orders Dataset

Records: 15,690

Columns:

* OrderID
* CustomerID
* ProductID
* Quantity
* Date and Time of Purchase
* Delivery Time
* Delivery Status

Purpose:
Sales transactions and order analysis.

---

### Products Dataset

Records: 80

Columns:

* ProductID
* Product Name
* Category
* Price
* Rating
* Number of People Rated the Product

Purpose:
Product performance and category analysis.

---

## Data Preparation

### Data Cleaning

Performed in Power Query:

* Checked for missing values
* Removed duplicate records
* Validated data types
* Standardized date formats
* Verified product prices
* Validated ratings
* Handled blank delivery times for cancelled orders

### Data Modeling

Relationships Created:

Customers[CustomerID] → Orders[CustomerID]

Products[ProductID] → Orders[ProductID]

Relationship Type:

One-to-Many

---

## DAX Measures

### Revenue

Revenue = Quantity × Product Price

### Total Orders

Count of all orders

### Average Order Value (AOV)

Revenue ÷ Total Orders

### Cancellation Rate

Cancelled Orders ÷ Total Orders

### Lost Revenue

Revenue from cancelled orders

---

## Dashboard KPIs

### Revenue

₹1.25 Billion

### Average Order Value

₹112.85K

### Cancellation Rate

29.72%

### Lost Revenue Due to Cancellation

₹525.42 Million

### Total Orders

15.69K

---

## Dashboard Insights

### Top Revenue Generating Products

* MacBook Air
* OnePlus 9
* Sony Headphones
* HP Pavilion
* Samsung Galaxy

### Top Revenue Categories

* Laptop
* Mobile
* Headphones

### Top Revenue States

* Maharashtra
* Gujarat
* Rajasthan

### Revenue Trend

Revenue remained relatively stable across the first three quarters but experienced a noticeable decline in the final quarter, indicating potential operational or demand-related issues.

### Cancellation Analysis

Nearly 30% of orders were cancelled, resulting in revenue losses exceeding ₹525 million.

This indicates opportunities to improve:

* Inventory management
* Delivery operations
* Customer satisfaction

---

## Business Impact

The dashboard enables stakeholders to:

* Monitor business performance in real time
* Identify top-performing products
* Understand regional demand patterns
* Reduce revenue loss from cancellations
* Improve inventory planning
* Support data-driven decision making

---

## Tools Used

* Power BI
* Power Query
* DAX
* Data Modeling
* CSV Datasets

---

## Author

Aditi Sanghi

B.Tech Information Technology

Data Analytics | Power BI | SQL | Python
