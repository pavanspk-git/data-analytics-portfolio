# Project 2 — Retail Sales Analysis (Excel, Superstore)

**Goal:** Analyze the Superstore dataset to uncover sales, profit, and shipping insights.  

## 🧹 Data Cleaning
- Removed duplicates (Order ID + Product Name)
- Handled missing values (numeric → 0, text → “Unknown” where needed)
- Converted dates into proper date formats
- Added helper columns:
  - **Year** (`=YEAR([@[Order Date]])`)
  - **Month** (`=TEXT([@[Order Date]],"MMM")`)
  - **Profit Margin** (`=IF([@[Sales]]=0,0,[@[Profit]]/[@[Sales]])`)
  - **Ship Days** (`=[@[Ship Date]]-[@[Order Date]]`)

## 📊 Analysis with PivotTables
- Sales by Year (trend chart)
- Profit by Category (bar/pie)
- Top 10 Products by Sales (value filter)
- Monthly Sales Trends (line chart)
- Average Ship Days by Region (average)

## 📂 Files
- `Superstore_Analysis.xlsx` → cleaned data + PivotTables
- `screenshots/` → dashboard and chart previews

## 🧰 Skills Demonstrated
Excel cleaning • PivotTables & Charts • Top 10 filters • Slicers • Dashboard creation
