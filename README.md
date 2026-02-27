# PowerBI_Exam_AndyHadulo  
### AdventureWorks Sales Analysis Dashboard (Power BI)

---

##  Project Overview

This project presents a comprehensive **Business Intelligence solution** developed using the **AdventureWorks Sales dataset**.

The objective was to design an end-to-end analytical workflow incorporating:

- Data preparation  
- Data modelling  
- Data visualisation  
- Dashboard deployment using Microsoft Power BI  

The final output is an interactive executive dashboard providing actionable business insights.

---

##  Approach and Methodology

### 1️ Data Import and Transformation

- Connected to AdventureWorks Excel file containing **7 core tables**
- Performed data cleaning using **Power Query Editor**
- Created calculated columns for:
  - Profit analysis
  - Sales categories
- Applied data quality filters (removed pre-2018 records)
- Handled missing values
- Removed duplicate records

---

### 2️ Data Modelling

- Designed a **Star Schema**
- Configured **Sales** as the central fact table
- Established relationships with dimension tables:
  - Customer
  - Product
  - Date
  - Region
- Developed Date hierarchy:

```
Year > Quarter > Month > Day
```

---

### 3️ Visualisation and Reporting

- Developed multiple report pages with **10+ interactive visuals**
- Enabled cross-filtering across visuals
- Implemented drill-down capabilities
- Applied consistent themes and accessible color schemes
- Integrated:
  - Running totals
  - Performance tracking metrics
  - KPI indicators

---

## Screenshots
<img width="975" height="513" alt="image" src="https://github.com/user-attachments/assets/3282b576-f922-45e1-8d8d-09e92539c777" />

###  Star Schema
Star schema showing relationships between fact and dimension tables.

### Sales Overview Report
<img width="975" height="552" alt="image" src="https://github.com/user-attachments/assets/998c4c60-276b-40ac-86a5-ebf8db58fa31" />

Comprehensive sales dashboard featuring:

- KPI cards with sales targets and running totals:
  - Total Sales
  - Total Orders
  - Total Quantity
- Sales Trend Over Time
- Sales by Product Category
- Revenue Contribution by Product Category
- Sales by Region


## Key Insights

###  Sales Performance
- **Total Revenue:** $97 million across all periods  
- **Peak Month:** May recorded the highest sales volume  
- **Top Market:** The United States generated the highest total sales  

---

###  Product Analysis
- **Top Category:** Bikes contributed 96% of total revenue  
- **Best Performing Product:** Touring-3000 Yellow, 62  
  - Revenue: $351,000  
- **Average Profit Margin:** 11%  
  - Bikes showed the highest profitability  

---

### Customer Behaviour
- The majority of customers are located in the United States  
- Bikes significantly outperform other product categories in all regions  

---

### Forecasting
- **6-Month Projection:** $206 million expected revenue  
- **Growth Trend:** Slow upward trajectory based on historical analysis  

---

## Challenges Faced and Solutions

### Challenge 1: Date Table Complexity  
**Issue:** Multiple date-related tables after transformation  

**Solution:**  
Maintained:
- Original Date table for relationships  
- Date Summary table for aggregations  

---

### Challenge 2: Relationship Ambiguity  
**Issue:** Multiple potential relationship paths between tables  

**Solution:**  
Designed a clean star schema with:
- Sales as the central fact table  
- Single active relationships  

---

### Challenge 3: DAX Performance  
**Issue:** Complex calculations slowed report performance  

**Solution:**  
Optimised DAX formulas using:
- `CALCULATE`
- Proper filter context handling
- Efficient measure design

---

## Limitations

- Historical data only (no real-time updates)
- Does not incorporate external market factors
- Based on the AdventureWorks sample dataset
- Simplified Row-Level Security (RLS)
- Linear forecasting model
- Geographic analysis limited to the region level
- No product lifecycle tracking
- Assumes a single currency environment

---

## Author

**Andy Hadulo**  
Power BI Practical Exam Submission
