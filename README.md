# 🚀 SQL Data Analytics Project

Welcome to my SQL Data Analytics Project! This repository is dedicated to extracting actionable business insights, tracking key performance indicators (KPIs), and performing deep-dive data analysis using advanced T-SQL.

![SQL Data Analytics Architecture](./docs/architecture.svg)

### 🔗 The Data Source
This project represents the analytical phase of my end-to-end data architecture. All queries and reports in this repository are executed against the **Gold Layer** (Fact and Dimension tables) that I built from scratch in my previous project. 

> **View the foundational data architecture here:** > [End-to-End SQL Data Warehouse Project](https://github.com/KrishnaSai315/sql-DataWarehouse_Project) *(This links to the ingestion, transformation, and dimensional modeling of the raw ERP and CRM data).*

---

## 🏗️ Analytics Architecture & Roadmap

![Project Roadmap](docs/Project%20Roadmap.png)

With the data successfully modeled into a Star Schema, the objective of this repository is to answer high-level business questions and empower stakeholders with data-driven reports. 

## 📊 Core Analytical Objectives

Based on the project requirements, I engineered complex SQL scripts to analyze three primary business domains:

### 1. Customer Analysis
Understanding who the customers are and how they interact with the business.
* **Demographic Profiling:** Analyzing distribution across age groups, genders, and geographic locations (countries).
* **Customer Segmentation:** Classifying customers into distinct categories (e.g., **VIP**, **Regular**, and **New**) based on their purchasing lifespan and total spending.
* **Behavioral Metrics:** Calculating average order values, average monthly spending, and customer recency.

### 2. Product Analysis
Evaluating inventory and catalog performance.
* **Category Performance:** Identifying which product categories and subcategories drive the most revenue.
* **Profitability & Costs:** Analyzing the average costs and pricing distributions across the product lines.
* **Performance Ranking:** Utilizing Window Functions to rank the top-performing and worst-performing products.

### 3. Sales & Trend Analysis
Tracking business growth and identifying seasonal patterns.
* **Time Series Analysis:** Aggregating sales by Year, Month, and Quarter to spot trends.
* **Cumulative Tracking:** Calculating running totals and moving averages to measure sustained growth.
* **Performance Benchmarking:** Implementing Year-over-Year (YoY) and Month-over-Month (MoM) comparisons to track increases or decreases in revenue.

---

## 🛠️ Tech Stack & SQL Techniques

- **Database Engine:** SQL Server
- **Core Tool:** SQL Server Management Studio (SSMS)
- **Advanced T-SQL Utilized:**
  - Common Table Expressions (CTEs) & Subqueries
  - Window Functions (`RANK()`, `DENSE_RANK()`, `ROW_NUMBER()`, `LAG()`, `OVER()`)
  - Aggregations (`SUM`, `COUNT`, `AVG`) & Grouping
  - Date and Time functions (`DATEDIFF`, `DATETRUNC`, `FORMAT`)
  - Conditional Logic (`CASE WHEN` statements for segmentation)

---

## 📂 Repository Structure

```text
├── datasets/                           # Processed Gold Layer datasets (CSV)
│   └── csv-files/                           # CSV files that contain Fact and Dimension tables used for analysis
│
├── docs/                               # Project roadmap and analytical requirement sketches
│
├── scripts/                            # Core analytical T-SQL scripts
│   ├── 01_database_exploration.sql     # Database structure and metadata exploration
│   ├── 02_dimensions_exploration.sql   # Distinct values and categorical analysis
│   ├── 03_date_range_exploration.sql   # Temporal boundaries analysis
│   ├── 04_measures_exploration.sql     # High-level aggregations and KPIs
│   ├── 05_magnitude_analysis.sql       # Distribution of metrics across dimensions
│   ├── 06_ranking_analysis.sql         # Top/Bottom N analysis using Window Functions
│   ├── 07_change_over_time_analysis.sql# Time-series and seasonal trends
│   ├── 08_cumulative_analysis.sql      # Running totals and moving averages
│   ├── 09_performance_analysis.sql     # YoY and MoM performance tracking
│   ├── 10_data_segmentation.sql        # Categorizing data into logical business segments
│   ├── 11_part_to_whole_analysis.sql   # Market share and proportion analysis
│   ├── 12_report_customers.sql         # Comprehensive customer reporting view
│   └── 13_report_products.sql          # Comprehensive product reporting view
│
└── README.md                           # Project overview

```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/KrishnaSai315/SQL-Data-Analytics/blob/main/LICENSE) file for details.

## Why I Built This Project
While my previous repository focused on the heavy backend engineering of building a Data Warehouse, I developed this project to showcase the other half of the equation: extracting actionable business value. I wanted to demonstrate my ability to step into a Business Intelligence role, write advanced, highly optimized T-SQL, and translate a pristine Star Schema into strategic insights that stakeholders can actually use to drive decisions.

## What I Accomplished Here

Executed Advanced T-SQL: Leveraged complex window functions, Common Table Expressions (CTEs), and dynamic aggregations to perform deep-dive analyses on Gold-layer data.

Engineered Strategic Segmentation: Categorized customers and products based on behavioral metrics, purchasing lifespans, and historical profitability to identify key drivers of business growth.

Delivered Performance Analytics: Built cumulative and time-series analyses (including Year-over-Year and Month-over-Month tracking) to uncover sales trends, benchmark performance, and provide a clear picture of overall business health.


