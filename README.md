# Adventure Works Sales Analysis Dashboard
### Power BI Report | FY 2023–2025 | By Aryan Rai

---

## Overview

This Power BI dashboard provides a comprehensive analysis of Adventure Works' sales performance across FY 2023–2025. It covers executive KPIs, product performance, customer behaviour, geographic distribution, profitability, and calendar-based trends — all designed to support data-driven business decisions.

| Metric | Value |
|--------|-------|
| Total Sales | $25M |
| Total Profit | $10M |
| Profit Margin | 41.96% |
| Total Returns | ~2K |
| Total Orders | 84,174 |

---

## Dashboard Preview

### Executive Overview
![Executive Overview](Executive_Overview.png)

### Category Analysis
![Category Analysis](Category_Analysis.png)

### Customer Analysis
![Customer Analysis](Customer_Analysis.png)

### Geographical Analysis
![Geographical Analysis](Geography_Analysis.png)

### Product Performance
![Product Performance](Product_Performance_Analysis.png)

### Profitability Analysis
![Profitability Analysis](Profitability_Analysis.png)

### Calendar Analysis
![Calendar Analysis](Calender_Analysis.png)

> 💡 **Note:** To view dashboard screenshots, click any PDF link above, or open `Adventure_Works .pdf` for the full report.

---

## Dashboard Pages

### 1. Executive Overview
High-level KPIs with year-wise trends for sales, cost, profit, and return rate.  
**Key Insight:** Sales grew from $6.4M (2023) to $9.3M (2024) while costs grew slower, improving efficiency. Profit margin rose from 40.62% to 42.53%.

### 2. Category Overview
Sales and profitability breakdown by product subcategory with MoM growth analysis.  
**Key Insight:** Road Bikes ($11.3M) and Mountain Bikes ($8.6M) dominate revenue. Accessory subcategories like Tires & Tubes and Helmets show high margins despite lower volume.

### 3. Customer Analysis
Customer segmentation by region, product category, year, and income level.  
**Key Insight:** Customer acquisition spiked in mid-2024. Southwest (4.1K) and Australia (3.5K) lead in customer concentration. Average income segment drives the most volume.

### 4. Geographical Analysis
Country and region-wise sales, orders, returns, and MoM growth.  
**Key Insight:** North America contributes 38.97% of sales. European markets show the highest MoM growth. Canada delivers the best profit margin efficiency.

### 5. Product Performance Analysis
Top products by sales, profit, margin, and return rate.  
**Key Insight:** Mountain-200 and Road-250 series are top performers. A small group of products drives the majority of revenue and profit.

### 6. Profitability Analysis
Detailed cost vs. profit breakdown by subcategory and region.  
**Key Insight:** Socks (66.67%), Helmets (63.64%), and Fenders (62.87%) lead on profit margin. Australia and Southwest lead in absolute profit; Canada leads in margin efficiency.

### 7. Calendar-Based Analysis
Monthly, weekday vs. weekend, and seasonal sales patterns.  
**Key Insight:** December saw a 50.56% MoM growth spike. 71.32% of sales occur on weekdays. Sales peaked in 2024 and stabilised in 2025.

---

## Tools & Technologies

| Tool | Usage |
|------|-------|
| Power BI Desktop | Dashboard development & visualisation |
| DAX | Calculated measures (MoM Growth, Profit Margin, Return Rate, etc.) |
| Power Query (M) | Data transformation & star schema modelling |
| Star Schema | Fact + Dimension table data model |

---

## Key DAX Measures Used

```dax
Total Sales = SUM(Sales[SalesAmount])
Total Profit = [Total Sales] - [Total Cost]
Profit Margin = DIVIDE([Total Profit], [Total Sales])
MoM Growth Rate = DIVIDE([Total Sales] - [Previous Month Sales], [Previous Month Sales])
Return Rate = DIVIDE([Total Returns], [Total Orders])
Previous Month Sales = CALCULATE([Total Sales], DATEADD('Date'[Date], -1, MONTH))
```

---

## Data Model

The report is built on a **Star Schema** with the following structure:

- **Fact Table:** Sales (orders, revenue, cost, returns)
- **Dimension Tables:** Product, Customer, Territory, Date/Calendar

---

## File Structure

```
Adventure_works_sales/
│
├── Adventure_Works.pbix                  # Main Power BI file
├── Adventure_Works .pdf                  # Full dashboard export (all 7 pages)
├── README.md                             # Project documentation
│
├── Executive_Overview.pdf                # Page 1 — KPIs & yearly trends
├── Category_Analysis.pdf                 # Page 2 — Subcategory sales & margins
├── Customer_Analysis.pdf                 # Page 3 — Customer segments & regions
├── Geographical_Analysis.pdf            # Page 4 — Country & region breakdown
├── Product_Performance_Analysis.pdf     # Page 5 — Product-level performance
├── Profitability_Analysis.pdf           # Page 6 — Cost vs profit by category
└── Calender_Analysis.pdf                # Page 7 — Monthly & seasonal trends
```

---

## How to Use

1. Open `Adventure_Works.pbix` in **Power BI Desktop** (May 2023 or later recommended).
2. Use the **Year** and **Region** slicers on each page to filter the data.
3. Navigate between pages using the bottom tab bar or page navigation buttons.
4. Hover over any visual for detailed tooltips.
5. Open `Adventure_Works .pdf` for a static export of all 7 pages, or open individual page PDFs for focused reference.

---

## Author

**Aryan Rai**  
BS Data Science — IIT Madras  
Data Analytics Certification — NDMIT Varanasi  
📧 aryanrai2555@gmail.com  
📞 9670262555  
🔗 [LinkedIn](https://www.linkedin.com/in/aryan-rai-590549310)

---

*Built as part of NDMIT Data Analytics Certification coursework.*
