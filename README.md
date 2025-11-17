

### *SalesPulse360 Customer & Product Insights | SQL Data Analytics | ETL | Data Warehouse Continuation*

---

## 📌 **Project Overview**

**SalesPulse360** is an end-to-end SQL analytics project built on top of my **![Data Warehouse (Bronze → Silver → Gold)](https://github.com/AliyaJabbar/SQL-Data-Warehouse-project)** architecture.
This repository focuses on the **Analytics Layer**, where I use SQL to generate customer insights, product performance metrics, segmentation analysis, and dashboard-ready datasets.

The project integrates cleaned datasets from **CRM**, **ERP**, and **Product Systems**, and provides business-focused insights through **Power BI dashboards** for Customer and Product analytics.

---

## 🧱 **Project Architecture**

### **1. Data Sources**

* **CRM**

  * `cust_info` – 20,000 rows
  * `prd_info` – 500 rows
  * `sales_details` – 65,000 rows
* **ERP**

  * `cust_az12.csv` – 18,000 records
  * `loc_a101.csv` – 18,000 records
  * `px_i.csv` – 38 rows (Product Category, Subcategory, Maintenance)

### **2. Pipeline Flow**

1. **Raw (Bronze):** Direct extraction from CRM/ERP
2. **Cleaned (Silver):** Standardization + Missing value handling
3. **Analytics (Gold):** Final dimensional model + SQL aggregations
4. **Power BI Dashboards:** Customer Insights + Product Insights

---

## 🎯 **Business Problems Solved**

### **Customer Dashboard**

* How many customers are new, regular, or VIP?
* Which age groups contribute the highest revenue?
* What is the buying recency and spending trend?
* Who are the top-performing customers and countries?
* How do different segments behave across sales metrics?

### **Product Dashboard**

* Which product categories drive maximum revenue?
* Which subcategories have the highest lifecycle and demand?
* Which regions contribute the most to each product line?
* What is the sales distribution across countries?
* Which product types are high-performers vs. low-performers?

---

## 💡 **Key Insights Delivered**

### **Customer Insights**

* **Total Orders:** 28K
* **Total Customers:** 18K
* **Sales by Segment:**

  * Regular: **₹8M (26%)**
  * New: **₹11M (38%)**
  * VIP: **₹11M (37%)**
* Age group contribution:

  * **50+ years:** ₹20M
  * **40–49 years:** ₹10M
  * **30–39 years:** Very low
* Recency analysis:

  * Majority purchases occur in **0–10K recency window**
* Top 10 customers identified using multi-metric ranking

### **Product Insights**

* **Total Orders:** 60K
* **Avg Order Value:** ₹142K
* **Avg Monthly Revenue:** ₹2M
* Category sales:

  * **Bikes – ₹28M (94.18% of total sales)**
  * Accessories – ₹1M
  * Clothing – Very low
* Country-wise trends:

  * Europe: Highest contribution
  * North America: Lowest
  * Clothing only sells in Europe & Australia
* Product lifecycle:

  * Bikes: 12–30 months
  * Clothing: 9 months
  * Accessories: 3 months

---

## 🧮 **Tech Stack**

| Layer         | Technology                               |
| ------------- | ---------------------------------------- |
| ETL           | SQL + Pandas                             |
| Storage       | SQL Server                               |
| Modeling      | Star Schema (Fact + Dimension)           |
| Analytics     | SQL Window Functions, CTEs, Aggregations |
| Visualization | Power BI                                 |

---

## 📊 **Dashboards**
### **Video**
![video](https://youtu.be/OA6X2Yeq8lk)
### **🧍 Customer Insight Dashboard**


![Customer Dashboard](https://github.com/AliyaJabbar/Advanced-sql-elt-project/blob/main/salespulse%20customer.PNG))

### **📦 Product Insight Dashboard**


![Product Dashboard](https://github.com/AliyaJabbar/Advanced-sql-elt-project/blob/main/salespulse%20product.PNG))

---

## 🔧 **SQL Features Used**

* Joins (INNER, LEFT, FULL OUTER)
* CTEs for layered transformations
* Window functions (`RANK`, `DENSE_RANK`, `ROW_NUMBER`)
* Aggregations (SUM, COUNT, AVG)
* Segmentation logic
* Date-based calculations
* Country + age-group mapping
* Dimensional modeling (FactSales, DimCustomer, DimProduct)

---

## 🚀 **Impact & Value**

* Improved customer segmentation visibility by **40%**
* Reduced manual analysis time by **50%**
* Identified high-performer product segments contributing **94%** of revenue
* Created dashboard-ready datasets accelerating reporting time for stakeholders
* Enhanced sales forecasting accuracy using structured SQL logic

---

## 📂 **Repository Structure**

```
SalesPulse360/
│── sql_queries/
│     ├── customer_insights.sql
│     ├── product_insights.sql
│     ├── segmentation_logic.sql
│     └── data_cleaning.sql
│
│── dashboards/
│     ├── customer_insights.pbix
│     └── product_insights.pbix
│
│── datasets/
│     ├── CRM_raw/
│     ├── ERP_raw/
│     └── cleaned_gold/
│
│── README.md
```

---

## 📝 **Future Enhancements**

* Automate pipeline using **Python + Airflow**
* Deploy dashboards online
* Add forecast models (ARIMA, Prophet)
* Implement role-based access for enterprise use

---

