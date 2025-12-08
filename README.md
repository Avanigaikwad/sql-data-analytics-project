# 📊 SQL Data Analytics Project

A complete end-to-end SQL analytics repository featuring EDA, advanced analytics, and business reporting.
___________________________________________________________________________________________________________

## 📘 Project Overview
This project demonstrates hands-on SQL analytics for a realistic retail sales dataset using:

Fact table : gold.fact_sales

Dimensions: gold.dim_products, gold.dim_customers

The goal of the project is to showcase core and advanced SQL skills used by Data Analysts, including:

✔ Data Exploration

✔ Business Metric Calculations

✔ Trend Analysis

✔ Ranking & Distribution Analysis

✔ Customer / Product Segmentation

✔ Creating BI-ready SQL Views

---
## 🧪 1. Exploratory Data Analysis (EDA)

File: exploratory_data_analysis.sql

This script covers:

- Database schema exploration
- Dimension profiling (products, customers, etc.)
- Date range and time-based analysis
- Key metric checks
- Category-level magnitude analysis
- Ranking (top/bottom performers)

Helps understand the dataset before deeper analytics.

---

## 📈 2. Advanced Analytics

File: advanced_analytics.sql

Includes advanced analytical patterns:

- Change Over Time: Yearly, monthly trends
- Cumulative Metrics: Running totals, moving averages
- Performance Analysis: YoY, average vs current, trend classification
- Part-to-Whole: Contribution % by category
- Segmentation:
  - Customer segments (VIP, Regular, New)
  - Product cost/sales segments

Uses functions such as LAG(), OVER(), DATETRUNC(), FORMAT(), CASE, etc.

---
## 📑 3. Project Report SQL Views
File: project_report.sql
It generates two BI-ready SQL reports:
### 🔹 Customer Report (gold.report_customers)
Includes:
- Age calculation & age-grouping
- Segmentation: VIP, Regular, New
- Metrics: total orders, total sales, quantity, lifespan
- KPIs:
  - Recency
  - Average Order Value
  - Monthly Spend

### 🔹 Product Report (gold.report_products)

Includes:
- Category & subcategory info
- Revenue-based product segmentation
- Metrics: total orders, customers, quantity sold
- KPIs:
  - Recency
  - Average order revenue
  - Monthly revenue

These views can be directly used in Power BI/Tableau dashboards.

## 📂 Repository Structure
```
 sql_data-analytics/
│
├── README.md
│
├── datasets/
│
├── sql/
│   ├── exploratory_data_analysis.sql      # Initial database exploration & profiling
│   ├── advanced_analytics.sql             # Advanced analytics: YoY, MoM, segmentation, etc.
│   ├── project_report.sql                 # Final business reports (customer + product)
│
├── docs/
│   ├── project_overview.pdf     # High-level documentation
│   └── ERD.drawio.png         # Entity Relationship Diagram
│
└── assets/
    └── screenshots/             # Images for visualizations or documentation
```
