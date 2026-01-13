# 🛍️ Customer Shopping Behavior Analysis

An end-to-end **Data Analytics project** demonstrating how raw customer transaction data can be transformed into actionable business insights using **Python, SQL (MySQL), and Power BI**.

---

## 📌 Project Overview

This project analyzes customer shopping behavior to identify:
- Revenue drivers across product categories
- Customer trends by age group and gender
- Subscription and shipping behavior patterns

The project follows a complete analytics lifecycle:
**Data Loading → Cleaning → EDA → SQL Analysis → Power BI Dashboard → Business Report**

---

## 📊 Dataset

- **File:** `customer_shopping_behavior.csv`
- **Format:** CSV
- **Description:**  
  Customer-level shopping data including demographics, product categories, purchase amounts, ratings, subscription status, and shipping types.

**Key Columns:**
- `Customer_ID`
- `Age_Group`
- `Gender`
- `Category`
- `Purchase_Amount`
- `Rating`
- `Subscription_Status`
- `Shipping_Type`

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|-----|--------|
| **Python (Pandas, NumPy, Matplotlib)** | Data cleaning & EDA |
| **MySQL** | Aggregations and insights |
| **Power BI** | Interactive dashboard & KPIs |
| **Jupyter Notebook** | Analysis & modeling |

---

## 🔍 Project Workflow

### 1️⃣ Data Loading & Exploratory Data Analysis (Python)
- Loaded raw CSV data using Pandas
- Checked data quality, distributions, and outliers
- Performed exploratory analysis on customer and revenue trends

---

### 2️⃣ Data Cleaning & Feature Engineering
- Handled missing and inconsistent values
- Standardized categorical variables
- Created derived fields for age groups and revenue analysis

---

### 3️⃣ SQL Analysis (MySQL)
- Imported cleaned data into MySQL
- Wrote SQL queries to answer business questions such as:
  - Revenue by product category
  - Sales by age group
  - Subscription vs non-subscription behavior

---

## 📊 Power BI Dashboard

Built an interactive dashboard featuring:
- KPI cards (Total Customers, Avg Purchase Amount, Avg Rating)
- Revenue by product category
- Revenue & sales by age group
- Subscription status distribution
- Dynamic filters for gender, category, and shipping type

📊 Dashboard Preview:
![Power BI Dashboard](<img width="1348" height="735" alt="image" src="https://github.com/user-attachments/assets/2a8b0299-3a77-487e-b347-7b2a35329f91" />)

---

## ⚠️ Common Issue: MySQL Connector for Power BI

When connecting **MySQL to Power BI**, users may face connection errors due to a **missing MySQL .NET connector**.

### 🔑 Solution
Power BI requires the **MySQL Connector/NET** to establish a connection.

➡️ Download the connector from: https://dev.mysql.com/downloads/connector/net/

---

> ⚠️ Important:
- Install the connector **before opening Power BI**
- Ensure the connector version matches your **Power BI (64-bit)** installation
- Restart Power BI after installation

---

## 🔗 Steps: Import Data from MySQL into Power BI

Follow these steps to connect Power BI to the MySQL database used in this project.

### 🗄️ Database Details
- **Server:** `localhost`
- **Port:** `3306`
- **Database:** `sales_db`
- **Table:** `customer`

---

### Step-by-Step Guide

1. Open **Power BI Desktop**
2. Click **Home → Get Data**
3. Select **MySQL database**
4. Enter the following details:
   - **Server:** `localhost`
   - **Database:** `sales_db`
5. Click **OK**
6. Enter your **MySQL username and password**
7. Choose **Database** authentication
8. Select the table:
9. Click **Load** (or **Transform Data** if further cleaning is needed)

✅ The data will now be available for building visuals and dashboards.

---

## ▶️ How to Run This Project

### 1. Clone the Repository
```
git clone https://github.com/your-username/customer-shopping-analysis.git
cd customer-shopping-analysis
```
### 2. Run Python Analysis
pip install pandas numpy matplotlib
jupyter notebook "data modeling.ipynb"

### 3. Run SQL Queries
Import cleaned data into MySQL
Execute:
insights.sql

### 4. Open Power BI Dashboard
Ensure MySQL Connector/NET is installed
Open the .pbix file
Refresh data to load from sales_db.customer

---

## 📄 Project Report
A detailed report summarizing methodology, analysis, and business insights: 
```Customer_Analysis_Report.pdf```

---
## ⭐ If you find this project useful, feel free to star the repository!
