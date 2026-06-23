# 📱 Mobile Sales Analytics Dashboard

An end-to-end Business Intelligence solution developed using **Microsoft Power BI** to analyze mobile sales performance across multiple business dimensions including brands, cities, customer behavior, payment methods, and historical sales trends.

---

## 🚀 Project Overview

The Mobile Sales Analytics Dashboard provides a centralized and interactive platform for monitoring business performance. The dashboard enables stakeholders to track KPIs, analyze sales trends, evaluate customer behavior, and make data-driven decisions.

---

## 🎯 Business Problem

The organization relied heavily on spreadsheet-based reporting, which resulted in:

- Lack of centralized reporting.
- Limited visibility into business performance.
- Time-consuming manual analysis.
- Difficulty in tracking historical trends.
- Inability to quickly identify top-performing products and regions.

To overcome these challenges, an interactive Power BI dashboard was developed.

---

## 🏆 Business Objectives

- Monitor overall sales performance.
- Analyze sales by brand, city, and product.
- Track Month-to-Date (MTD) sales.
- Compare current performance with previous periods.
- Understand customer purchasing behavior.
- Identify top-performing regions and products.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|---------|
| Power BI Desktop | Dashboard Development |
| Power Query | ETL & Data Transformation |
| DAX | Business Calculations |
| Excel | Data Source |
| Power BI Service | Deployment |

---

## 📂 Dataset Information

- **Source:** Microsoft Excel (.xlsx)
- **Records:** 3,835 Transactions
- **Columns:** 14
- **Granularity:** One row represents one sales transaction.

### Dataset Attributes

- Transaction ID
- Day
- Month
- Year
- Day Name
- Brand
- Mobile Model
- Units Sold
- Price Per Unit
- Customer Name
- Customer Age
- City
- Payment Method
- Customer Ratings

---

# 🔄 ETL Process

## Extract

- Imported raw sales data from Excel into Power BI.

## Transform

Data preprocessing was performed using **Power Query**.

### Data Cleaning Activities

✔ Checked missing values

✔ Validated duplicate records

✔ Corrected data types

✔ Standardized categorical values

✔ Renamed columns

✔ Validated data consistency

### Feature Engineering

Created additional analytical structures:

- Date Hierarchy
- Calendar Table
- Month-Level Analysis
- Day-Level Analysis

## Load

Cleaned and transformed data was loaded into the Power BI semantic model.

---

## 📊 Data Quality Checks

| Check | Status |
|--------|--------|
| Null Value Validation | Completed |
| Duplicate Check | Completed |
| Data Type Validation | Completed |
| Consistency Validation | Completed |
| Categorical Validation | Completed |

---

## 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Brand-wise Sales Analysis
- City-wise Sales Analysis
- Product Performance Analysis
- Customer Rating Analysis
- Payment Method Analysis
- Monthly Trend Analysis
- Day-wise Sales Analysis

---
## 🏗️ Data Modeling

A dimensional modeling approach was implemented.

### Fact Table

- `Fact_Mobile_Sales`

### Dimension Table

- `Dim_Calendar`

### Relationship

```text
Dim_Calendar[Date]
         │
         │ 1 : *
         │
Fact_Mobile_Sales[Date]
```

---

## 📷 Dashboard Preview

---

## 1. Executive Dashboard

<img src="Dashboard%20Preview.jpg" width="1000">

### Purpose

The Executive Dashboard provides a comprehensive overview of organizational sales performance, enabling stakeholders to monitor critical KPIs and business trends.

### Key Visuals

- KPI Cards (Total Sales, Quantity Sold, Transactions, Average Price)
- Sales by City Map
- Monthly Quantity Trend
- Customer Rating Analysis
- Payment Method Distribution
- Brand Performance Matrix
- Top Selling Mobile Models

### Key Insights

- Apple emerged as the highest revenue-generating brand.
- Metropolitan cities contributed significantly to total sales.
- Customers predominantly preferred digital payment methods.
- Customer satisfaction remained largely positive across transactions.

### Business Value

Provides executives with a centralized analytical view for strategic decision-making and business performance monitoring.

---

## 2. Month-To-Date (MTD) Dashboard

<img src="MTD%20Report.jpg" width="1000">

### Purpose

The MTD dashboard tracks cumulative sales performance within a selected month and helps monitor short-term business performance.

### Key Visuals

- Daily Cumulative Sales Trend
- Dynamic Month and Year Filters
- MTD Sales Analysis

### Key Insights

- Sales demonstrated a steady upward trend throughout the month.
- Month-end cumulative sales reached approximately 23 million.
- The selected period exhibited stable sales growth with no major fluctuations.

### Business Value

Enables business users to track monthly targets and proactively identify performance deviations.

---

## 3. Same Period Last Year Dashboard

<img src="Same%20Period%20Last%20Year%20report.jpg" width="1000">

### Purpose

The Same Period Last Year dashboard compares current sales performance with the corresponding period from the previous year to evaluate business growth.

### Key Visuals

- Year-over-Year Comparison
- Quarterly Sales Comparison
- Monthly Sales Comparison
- Historical Trend Analysis

### Key Insights

- Current year sales were marginally lower than previous year's sales.
- Quarterly performance remained relatively stable.
- Historical comparisons highlighted months requiring additional business investigation.

### Business Value

Supports strategic planning by enabling stakeholders to evaluate historical performance trends and measure business growth.

---
