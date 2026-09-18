# Retail Sales & Profitability Analytics Dashboard

An end-to-end Excel data analysis project — from raw, messy sales data to a fully interactive, dual-page dashboard with KPIs, charts, slicers, and business insights.

## 📌 Project Overview

This project analyzes retail sales data (1,000+ orders) across three product categories — Furniture, Office Supplies, and Technology — to uncover sales trends, regional performance, and profitability drivers. The raw dataset contained typical real-world data quality issues, which were cleaned and transformed before building the final dashboards.

## 🎯 Objective

To help the business understand:
- Which categories, regions, and segments generate the most sales and profit
- How sales trend over time (2023–2025)
- Which products and sub-categories are top performers
- How discounts and shipping preferences impact the business

## 🛠️ Tools Used

- Microsoft Excel (Pivot Tables, Charts, Slicers, Formulas)
- Data Cleaning (manual + formula-based)

## 📂 Project Structure

├── Raw_Data -> Original, uncleaned dataset (1,071 rows)
├── Clean_Data -> Cleaned dataset (1,050 rows) ready for analysis
├── Cleaning_Log -> Documented list of every cleaning step applied
├── Pivot_Analysis -> Pivot tables for Sales and Profit by Category, Region, Segment, Sub-Category, Month, and Top Products
├── Sales_Overview_Dashboard -> KPIs + charts for sales performance
└── Profit_Analysis_Dashboard -> KPIs + charts for profitability performance

## 🧹 Step 1: Data Cleaning

The raw dataset contained common real-world data issues, all of which were identified and resolved:

- Removed duplicate rows and duplicate Order IDs
- Standardized inconsistent text values (e.g., "east", "EAST", "Souht" → "East")
- Trimmed extra whitespace from text fields
- Converted inconsistent date formats into a single standard format
- Fixed negative values in Quantity and Sales (data entry errors)
- Handled missing values:
  - Missing Discount → filled with 0
  - Missing Unit Price → filled with category median
  - Missing Region/Segment → labeled "Unknown"
  - Missing Customer Name → labeled "Unknown Customer"
  - Missing Ship Date → estimated as Order Date + 3 days
- Recalculated Sales and Profit fields for consistency after cleaning

Full step-by-step log is documented in the Cleaning_Log sheet.

## 📊 Step 2: Pivot Tables

Separate pivot tables were built for Sales and Profit to analyze the data from multiple angles:
- Sales by Category
- Profit by Category and Sub-Category
- Sales by Region / Profit by Region
- Profit by Segment
- Monthly sales trend (2023–2025)
- Top 10 products by sales / Top 10 sub-category products by profit

## 📈 Step 3: Dashboard Design

Built two connected dashboards, linked with navigation buttons for quick switching.

### 1. Sales Overview Dashboard
KPIs: Total Sales, Total Quantity, Total Orders, Average Order Value

Charts:
- Sales by Month (trend line, 2023–2025)
- Sales by Category (bar)
- Sales by Region (pie)
- Top 10 Products by Sales (bar)

### 2. Profit Analysis Dashboard
KPIs: Total Profit, Profit Margin %, Average Discount

Charts:
- Top 10 Sub-Category Products by Profit (bar)
- Profit by Segment (pie)
- Profit by Region (pie)
- Profit by Category (bar)

Both dashboards include:
- Slicers (Category, Region, Segment, Ship Mode) for interactive filtering
- A consistent color theme (blue for Sales, green/olive for Profit) for visual distinction
- Navigation buttons to switch between dashboard pages

## 🔍 Key Insights

- Technology is the most profitable category ($145K profit), followed closely by Furniture ($125K). Office Supplies underperforms by comparison ($15K profit) and may need a revised strategy.
- East is the strongest performing region for both sales ($318K) and profit ($95.6K); West and North have room for growth.
- Home Office is the top-generating customer segment by profit ($113K), suggesting a strong work-from-home customer base.
- Copiers are the top sub-category by profit, followed by Sofas and Machines.
- Customers show a fairly even preference across shipping modes, with First Class and Same Day slightly ahead.
- The business maintains a stable ~30% profit margin overall.

## 📎 How to Use

1. Download the .xlsx file from this repository
2. Open in Microsoft Excel (2016 or later recommended for full slicer/chart support)
3. Use the navigation button on each dashboard to switch between Sales Overview and Profit Analysis
4. Use the slicers (Category, Region, Segment, Ship Mode) to filter the data interactively

## 👤 Authur 

Kiran Analyst



##  Dashboard Preview

### Sales Analysis Dashboard
![Sales Analysis Dashboard](Sales%20Analysis%20Dashboard.png)

### Profit Analysis Dashboard
![Profit Analysis Dashboard](Profit%20Analysis%20Dasboard%20.png)
