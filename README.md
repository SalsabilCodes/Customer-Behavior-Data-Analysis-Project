# 📊 Customer Behavior Data Analysis Project

This project represents a **complete, industry-standard, end-to-end data analytics workflow**, designed to mirror the responsibilities of professional analysts in modern business environments. The project covers all critical stages of data analysis, from data preparation and modeling to insight generation, visualization, and reporting.

---

## 1️⃣ Project Overview

The goal of this project is to simulate a corporate-grade **end-to-end data analytics workflow**, demonstrating the ability to translate raw data into strategic business intelligence by:

- **Data Preparation, Modeling & Exploratory Data Analysis (Python):** Clean and transform the raw dataset for analysis.  
- **Data Analysis (SQL):** Simulate business transactions and run queries to extract insights on customer segments, loyalty, and purchase drivers.  
- **Visualization & Insights (Power BI):** Build an interactive dashboard highlighting key patterns and trends, enabling stakeholders to make data-driven decisions.  
- **Report & Presentation:** Write a clear project report summarizing key findings and recommendations. Prepare a visual presentation for stakeholders.

**Business Problem Statement:**  
A leading retail company wants to better understand its customers’ shopping behavior to improve **sales, customer satisfaction, and long-term loyalty**. Management noticed changes in purchasing patterns across demographics, product categories, and sales channels (online vs. offline).  

> Overarching Business Question:  
> “How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?”

---

## 2️⃣ Dataset Summary

- **Rows:** 3,900  
- **Columns:** 18  
- **Key Features:**
  - **Customer demographics:** Age, Gender, Location, Subscription Status  
  - **Purchase details:** Item Purchased, Category, Purchase Amount, Season, Size, Color  
  - **Shopping behavior:** Discount Applied, Promo Code Used, Previous Purchases, Purchase Frequency, Review Rating, Shipping Type  
- **Missing Data:** 37 values in Review Rating column  
- **Dataset Source:** [GitHub CSV](https://github.com/amlanmohanty1/customer-trends-data-analysis-SQL-Python-PowerBI/blob/main/customer_shopping_behavior.csv)

---

## 3️⃣ Exploratory Data Analysis (Python)

- **Data Loading:** Imported dataset using Pandas  
- **Initial Exploration:** `.info()` and `.describe()`  
- **Missing Data Handling:** Imputed missing `Review Rating` values using median per product category  
- **Column Standardization:** Converted to snake_case for clarity  
- **Feature Engineering:**  
  - `age_group` column created by binning customer ages  
  - `purchase_frequency_days` from purchase data  
- **Data Consistency Check:** Verified `discount_applied` vs `promo_code_used`; dropped redundant column  
- **Database Integration:** Connected to PostgreSQL and loaded cleaned data for SQL analysis

---

## 4️⃣ Data Analysis (SQL)

Performed structured analysis in PostgreSQL to answer business questions:

1. **Revenue by Gender:** Compare revenue of male vs female customers  
2. **High-Spending Discount Users:** Identify customers using discounts but spending above average  
3. **Top 5 Products by Rating:** Products with highest average review ratings  
4. **Shipping Type Comparison:** Average purchase by Standard vs Express shipping  
5. **Subscribers vs Non-Subscribers:** Compare spend and revenue  
6. **Discount-Dependent Products:** Top 5 products with highest percentage of discounted purchases  
7. **Customer Segmentation:** New, Returning, Loyal  
8. **Top 3 Products per Category:** Most purchased products within each category  
9. **Repeat Buyers & Subscriptions:** Customers with >5 purchases and subscription likelihood  
10. **Revenue by Age Group:** Total revenue contribution by age group  

> SQL queries are saved in `customer_behavior_sql_queries.sql`

---

## 5️⃣ Dashboard (Power BI)

- Connected SQL database to Power BI  
- Created **interactive dashboard** displaying insights such as:  
  - Revenue by demographics  
  - Customer segments  
  - Top products by rating and sales  
  - Discount & subscription trends  

> Dashboard file: `customer_behavior_dashboard.pbix`

---

## 6️⃣ Business Recommendations

- **Boost Subscriptions:** Promote exclusive subscriber benefits  
- **Customer Loyalty Programs:** Reward repeat buyers and move them to the “Loyal” segment  
- **Review Discount Policy:** Balance sales increase with margin control  
- **Product Positioning:** Highlight top-rated and best-selling products  
- **Targeted Marketing:** Focus on high-revenue age groups and express-shipping users  

---

## 7️⃣ Project Deliverables

1. **Data Preparation & Modeling (Python)** – Cleaned and transformed dataset  
2. **Data Analysis (SQL)** – Structured queries extracting key insights  
3. **Visualization & Insights (Power BI)** – Interactive dashboard  
4. **Report & Presentation** – Summary report and slide deck with insights  
5. **GitHub Repository** – Python scripts, SQL queries, dashboard, and documentation  

---

## 8️⃣ Folder Structure (Example)
