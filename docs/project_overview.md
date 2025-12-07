# Project Overview – Retail Sales Data Analytics
## 1. Introduction
This document provides a high-level overview of the **Retail Sales SQL Analytics Platform**, an end-to-end analytical solution designed for performing **Exploratory Data Analysis (EDA), advanced analytics, and BI reporting** using a structured SQL workflow.

The project demonstrates how SQL can be used to build reusable analytical assets, support business decision-making, and generate BI-ready datasets for dashboards.

## 2. Data Architecture

The analytical model follows a **fact–dimension (star schema)** structure:

- **Fact Table**

gold.fact_sales: Transaction-level sales data

- **Dimension Tables**

<span style="color:blue"> *gold.dim_products* </span?> : Product details, categories, costs

gold.dim_customers: Customer demographics and attributes

This schema enables efficient metric calculations, time-series aggregation, and multi-level drill-downs.

## 3. Project Objectives

The primary objectives of this analytics platform are:

To showcase the use of SQL for end-to-end data analysis

Enable analysts to perform:

Data exploration and profiling

Business metric calculations

Trend and performance evaluations

Customer and product segmentation

Create reusable SQL views that can directly feed BI tools such as Power BI or Tableau

4. Key Components

The project is organized into three core analytical modules.
Each module is independent and reusable.

4.1 Exploratory Data Analysis (EDA)

File: exploratory_data_analysis.sql

This component focuses on understanding and validating the dataset before performing deeper analytics. It includes:

Schema and metadata inspection

Profiling product and customer dimensions

Time range and completeness checks

Category-level distribution analysis

Initial KPI computation

Identification of top / bottom performers

Outcome:
A clear understanding of data quality, structure, and initial trends.

4.2 Advanced Analytics

File: advanced_analytics.sql

This module applies advanced SQL patterns to extract meaningful business insights:

Time-Series Analysis

Monthly and yearly trend calculations

MoM and YoY growth metrics

Running totals and moving averages

Performance Analysis

Contribution analysis (category share %)

Performance vs. historical average

Trend classification using conditional logic

Segmentation Models

Customer segmentation: VIP, Regular, New

Product segmentation using cost or revenue tiers

Outcome:
A deeper understanding of customer behavior, product performance, and overall business health.

4.3 BI-Ready Reporting Views

File: project_report.sql

Generates two persistent analytical datasets for BI dashboards:

Customer Report – gold.report_customers

Includes:

Age calculation and age-banding

Order and revenue metrics

Recency and customer lifespan

AOV (Average Order Value)

Monthly spend trends

Customer segmentation (VIP / Regular / New)

Product Report – gold.report_products

Includes:

Category and subcategory details

Revenue-based product segmentation

Quantity and revenue metrics

Customer count per product

Recency and monthly revenue patterns

Outcome:
Ready-to-use datasets for visualization tools, ensuring consistent business metrics across teams.

5. Technical Highlights

Reusable modular SQL scripts

Use of window functions (LAG, LEAD, OVER)

Advanced date and time handling

Analytical functions for percentile/ranking

Dimensional modelling best practices

BI-optimized output tables

6. Intended Users

This documentation is designed for:

Data Analysts

BI Developers

Data Engineers

Students learning SQL analytics

Anyone building analytics projects with SQL

7. Summary

This project demonstrates a full SQL-based analytics pipeline—from raw data exploration to advanced analytics and BI reporting. The modular scripts, star-schema approach, and analytical views make the platform scalable, reusable, and suitable for real-world analytics use cases.
