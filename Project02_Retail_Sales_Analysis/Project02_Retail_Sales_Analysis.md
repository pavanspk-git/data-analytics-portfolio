# Project 2 — Retail Sales Analysis (Excel, Superstore)

## 📊 Overview
Excel-based analysis of the Superstore dataset. I cleaned the data, added helper columns (Year, Month, Profit Margin, Ship Days), and built PivotTables + charts (e.g., Sales by Year, Profit by Category, Top 10 Products, Avg Ship Days by Region).

## 🧹 Cleaning Summary
- Removed true duplicate rows (Order ID + Product Name).
- Handled missing values (numeric → 0; categorical → “Unknown” where appropriate).
- Converted **Order Date/Ship Date** to real dates; fixed numeric types for Sales/Profit/Quantity/Discount.
- Standardized text (TRIM) and created helper columns:
  - `Year = YEAR([@[Order Date]])`
  - `Month = TEXT([@[Order Date]], "MMM")`
  - `Profit Margin = IF([@[Sales]]=0, 0, [@[Profit]]/[@[Sales]])`
  - `Ship Days = [@[Ship Date]] - [@[Order Date]]`

## 📈 PivotTables & Charts
- **Sales by Year** (Column Chart)
- **Profit by Category** (Bar/Pie)
- **Monthly Sales Trend** (Line; Month in Rows, Year in Columns)
- **Top 10 Products by Sales** (Value Filter → Top 10)
- **Average Ship Days by Region**

> Tip inside Excel: Right‑click Pivot → **Value Field Settings** to switch Sum ↔ Average; use **Insert → Slicer** for Segment/Region/Category.

## 🗂 Files
- `Superstore_Analysis.xlsx` — cleaned data + PivotTables + charts in one workbook
- `README.md` — this file
- *(Optional)* `images/` — screenshots of dashboard/charts to preview in GitHub

## 🔁 How to Reproduce
1. Download Superstore dataset (Kaggle/Tableau sample).
2. Clean as described above; add helper columns.
3. Build PivotTables; apply **Top 10** filter for products/customers as needed.
4. Insert charts and arrange on a Dashboard sheet.
5. Save as `Superstore_Analysis.xlsx`.

## 🧪 Key Insights (examples; confirm with your data)
- Technology category often leads profit; Furniture may lag due to discounts.
- Strong Q4 seasonality (Nov–Dec peaks) in Sales.
- Ship Days typically 1–5; longer tails in certain regions.

## 🧰 Skills Demonstrated
Excel data cleaning • PivotTables & PivotCharts • Slicers • Business KPI design • Retail analytics

---

### How to view
Download `Superstore_Analysis.xlsx` and open in Microsoft Excel (Windows).