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

### Executive Dashboard

<img src="Dashboard%20Preview.jpg" width="1000">

---

### Month-To-Date (MTD) Dashboard

<img src="MTD%20Report.jpg" width="1000">

---

### Same Period Last Year Dashboard

<img src="Same%20Period%20Last%20Year%20report.jpg" width="1000">

---
