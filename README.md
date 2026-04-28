# 📊 Sales Performance Dashboard — Power BI

![Dashboard Preview]("<img width="1373" height="769" alt="Sales-Trends" src="https://github.com/user-attachments/assets/19018698-9661-4cfb-98a7-6f44ae5d955f" />
")

A multi-page interactive **Sales Performance Dashboard** built in Power BI to track key business metrics. Covers end-to-end sales analysis — from high-level revenue summaries to granular product, customer, region, and team-level breakdowns — with dynamic date slicers and cross-page filters.

---

## 🎯 Project Objective

> Build a **Sales Performance Dashboard** in Power BI to help Sales Managers, Business Executives, and Marketing Teams monitor, analyse, and act on key business metrics in real time.

### 👥 Target Users
- Sales Managers
- Business Executives
- Marketing Teams

### ✅ Dashboard Features Delivered
- Sales Overview
- Monthly & Yearly Sales Trends
- Top Customers & Products
- Profit & Revenue Analysis
- Dynamic Filters (Date, Region, Category)

### 📂 Data Sources
| Source | Format |
|--------|--------|
| Sales Transactions | Excel / SQL / CSV |
| Product Details | Excel / SQL / CSV |
| Customer Information | Excel / SQL / CSV |

---

## 📁 Repository Structure

```
sales-analytics-powerbi/
│
├── report.pbit                  # Power BI template (no embedded data)
├── README.md                    # This file
│
├── screenshots/
│   ├── summary.png
│   ├── profit-revenue-month.png
│   ├── profit-revenue-product.png
│   ├── sales-trends.png
│   ├── customer-product-summary-1.png
│   ├── customer-product-summary-2.png
│   └── profit-by-category-region.png
│
├── data/
│   └── sample_sales_data.csv    # Anonymised sample dataset
│
└── docs/
    ├── data-dictionary.md       # Column definitions
    └── dax-measures.md          # All DAX measure formulas
```

---

## 📄 Dashboard Pages

### 1. Summary
> **File:** `screenshots/summary.png`

The landing page giving a bird's-eye view of overall business performance.

| KPI | Value |
|-----|-------|
| Total Sale | 35,81,535 |
| Total Quantity Sold | 3,482 |
| Total Orders | 640 |
| Total Customers | 500 |
| Repeated Customers | 376 |

**Visuals included:**
- Total Sale by Date (line + area chart)
- Total Sale by Product (donut chart)
- Total Quantity Sold and Total Orders by Date (clustered bar)
- Repeated Customer and Repeated Customer % by Date (combo chart)

---

### 2. Profit and Revenue Sales — Monthly View
> **File:** `screenshots/profit-revenue-month.png`

Tracks monthly sales and profit performance with cumulative trend bars.

| KPI | Value (South, Team A) |
|-----|-----------------------|
| Total Sale | 35,81,5... |
| Profit Margin % | 30.00% |
| Profit | 1,074.4... |
| Average Revenue | 9.53K |

**Visuals included:**
- Total Sale by Month (line + area)
- Profit Margin % by Month (line + area)
- Cumulative Sales by Month (bar chart)
- Cumulative Profit by Month (bar chart)

---

### 3. Profit and Revenue Sales — Product View
> **File:** `screenshots/profit-revenue-product.png`

Breaks down profitability at the product level using contribution margin and variable cost comparisons.

**Visuals included:**
- Contribution Margin % by Product (pie chart — all products at 10% equal share)
- Profit Margin % by Product (line chart)
- Total Sale vs Total Variable Cost by Product (clustered bar)
- Total Sale, Variable Cost, and Sum of Profit by Product (combo chart)

---

### 4. Sales Trends
> **File:** `screenshots/sales-trends.png`

Month-over-month performance analysis for South region, Corporate segment, Team B.

**Visuals included:**
- Total Sale by Month (line + area)
- Total Orders by Month (line + area)
- Profit Margin % by Month (line + area)
- Sales Growth % by Month (line + area with negative values)

---

### 5. Customer and Product Summary — Overview
> **File:** `screenshots/customer-product-summary-1.png`

Ranks customers and products by total sales volume across all filters.

| Highlight | Value |
|-----------|-------|
| Most Selling Product | Monitor (Qty: 5,868) |
| Least Selling Product | Speaker (Qty: 5,270) |
| Top Customer | Customer 376 (2,11,656) |

---

### 6. Customer and Product Summary — Filtered View
> **File:** `screenshots/customer-product-summary-2.png`

Same page filtered to South region, Online segment (3 years).

| Highlight | Value |
|-----------|-------|
| Most Selling Product | Monitor (Qty: 403) |
| Least Selling Product | Printer (Qty: 312) |
| Top Customer | Customer 299 (67,142) |

---

### 7. Profit and Total Sale by Category, Region, Segment & Team
> **File:** `screenshots/profit-by-category-region.png`

Comparative clustered bar charts across all business dimensions.

| Dimension | Leader | Total Sale |
|-----------|--------|------------|
| Category | Accessories | 3,29,14,791 |
| Segment | Wholesale | 1,41,39,643 |
| Region | South | 1,46,01,838 |
| Team | Team B | 1,44,94,408 |

---

## 🔍 Key Insights

### 💰 Revenue & Profitability
- **Profit margin is consistently 30%** across all months, products, regions, and segments — indicating a fixed-margin pricing model or standardised cost structure.
- **Accessories outperform Electronics** significantly in total sales (3.29 Cr vs 2.35 Cr), suggesting accessories drive the majority of revenue volume.
- **All four regions perform within a tight band** (1.36 Cr – 1.46 Cr), showing balanced geographic coverage with South holding a slight lead.

### 📦 Product Performance
- **Monitor is the top-selling product** by quantity (5,868 units overall), while **Speaker is the least selling** (5,270 units) — a narrow gap suggesting fairly uniform product demand.
- **Smartphone leads in total sales value** despite not topping quantity charts, hinting at a higher unit price.
- **Equal contribution margins (10% each)** across all products confirms uniform pricing strategy.

### 👥 Customer & Segment
- **376 out of 500 customers are repeat buyers (75.2%)** — an exceptionally high retention rate, pointing to strong customer loyalty.
- In the **Online segment (South)**, Webcam overtakes Monitor as the top product, showing channel-specific demand patterns.
- **Wholesale segment leads** in total sales, barely ahead of Retail and Online — segments are nearly equally weighted.

### 📈 Sales Trends
- **Peak sales occurred in June 2023** (1,52,344) for the Corporate/South/Team B view, followed by a sharp dip in July — likely seasonal or campaign-driven.
- **Sales Growth % is highly volatile**, swinging from +99% (April) to -60% (August), suggesting inconsistent order patterns rather than steady organic growth.
- **Cumulative sales and profit curves are smooth and upward**, confirming overall healthy growth even with month-to-month fluctuations.

### 🏆 Team Performance
- **Team B leads all teams** in both profit and total sale (1,44,94,408), followed closely by Team D, Team C, and Team A — performance is tightly clustered within a ~5% range.

---

## 🛠️ Filters Available

All dashboard pages support the following interactive filters:

| Filter | Options |
|--------|---------|
| Date | Dynamic — Last N Days / Months / Years (Calendar or Fiscal) |
| Region | South, East, North, West |
| Segment | Wholesale, Retail, Online, Corporate |
| Team | Team A, Team B, Team C, Team D |

---

## 📐 Key Metrics & DAX Calculations

All measures are defined in Power BI using DAX. The table below mirrors the project's official metrics specification.

| Metric Name | Formula / Calculation | Description |
|-------------|----------------------|-------------|
| `Total Sales` | `SUM(SalesAmount)` | Total revenue generated |
| `Total Orders` | `COUNT(OrderID)` | Total number of sales orders |
| `Total Quantity Sold` | `SUM(Quantity)` | Total units sold |
| `Average Order Value` | `DIVIDE(SUM(SalesAmount), COUNT(OrderID))` | Average revenue per order |
| `Profit` | `SUM(SalesAmount - CostPrice * Quantity)` | Net earnings after cost |
| `Profit Margin %` | `DIVIDE(SUM(SalesAmount - CostPrice * Quantity), SUM(SalesAmount)) * 100` | Profitability percentage |
| `Sales Growth %` | `((CurrentPeriodSales - PreviousPeriodSales) / PreviousPeriodSales) * 100` | Sales increase/decrease over time |
| `Top 5 Products` | `TOPN(5, SUM(SalesAmount))` | Best-performing products |
| `Top 5 Customers` | `TOPN(5, SUM(SalesAmount), CustomerName)` | Most valuable customers |
| `Sales by Region` | `SUM(SalesAmount) GROUP BY Region` | Sales distribution across regions |
| `Monthly Sales Trend` | `SUM(SalesAmount) BY Month` | Sales trends over time |
| `Returning Customers %` | `DIVIDE(COUNT(DISTINCT(RepeatCustomerID)), COUNT(DISTINCT(CustomerID))) * 100` | Percentage of customers making repeat purchases |

> Full DAX formulas with context filters are documented in [`docs/dax-measures.md`](docs/dax-measures.md)

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `report.pbit` in **Power BI Desktop**
3. When prompted, connect your data source (CSV or database) matching the schema in `docs/data-dictionary.md`
4. Refresh the data and publish to Power BI Service if needed

---

## 📋 Data Schema (Summary)

| Column | Type | Description |
|--------|------|-------------|
| `Date` | Date | Transaction date |
| `CustomerName` | Text | Customer identifier |
| `Product` | Text | Product name |
| `Category` | Text | Accessories or Electronics |
| `Region` | Text | South / East / North / West |
| `Segment` | Text | Wholesale / Retail / Online / Corporate |
| `Team` | Text | Sales team (A–D) |
| `TotalSale` | Decimal | Revenue from transaction |
| `VariableCost` | Decimal | Cost of goods |
| `Profit` | Decimal | TotalSale − VariableCost |
| `Quantity` | Integer | Units sold |
| `Orders` | Integer | Number of orders |

> Full column definitions in [`docs/data-dictionary.md`](docs/data-dictionary.md)

---

## 📌 Notes

- `.pbix` file is **excluded** from this repository as it contains embedded data. Only the `.pbit` template is shared.
- All screenshots are taken with sample/anonymised data.
- Indian number formatting is used throughout (e.g. 35,81,535 = 3.58 million).

---

## 🤝 Author

Built as a portfolio project demonstrating Power BI skills including data modelling, DAX, interactive filtering, and multi-page dashboard design.
