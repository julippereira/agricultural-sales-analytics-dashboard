# 📊 Power BI Report

This directory contains the Power BI report developed for the Agricultural Sales Analytics Dashboard project.

---

## Report File

```text
power_bi/
└── Agricultural_Sales_Analytics.pbix
```

---

## Dashboard Overview

The report provides an interactive environment for analyzing commercial performance across customers, products, brands, regions, and time periods.

Key analytical areas include:

### Revenue Overview

- Total Revenue
- Revenue Trends
- Monthly Performance
- Annual Comparison
- Revenue Growth

### Portfolio Analysis

- Product Performance
- Category Analysis
- Brand Comparison
- Product Rankings

### Customer Analytics

- Top Customers
- Bottom Customers
- Purchase Volume Analysis
- Revenue Contribution

### Geographic Analysis

- Revenue by State
- Revenue by Sales Region
- Revenue by Sales Management Area

---

## Data Model

The report uses a star schema design.

```text
                 Calendar
                     │
                     │
Customers ─── Sales Fact ─── Products
                     │
                     │
                Categories
```

---

## Features

- Interactive slicers
- KPI cards
- Time intelligence calculations
- Revenue analysis
- Ranking analysis
- Geographic visualizations
- Cross-filtering
- Drill-down navigation

---

## Main Technologies

- Power BI Desktop
- DAX
- Power Query
- Star Schema Modeling

---

## Sample Metrics

```DAX
Revenue =
SUMX(
    Sales,
    Sales[Quantity Sold] *
    Sales[Unit Price]
)
```

```DAX
Revenue YTD =
TOTALYTD(
    [Revenue],
    Calendar[Date]
)
```

```DAX
Revenue Growth % =
DIVIDE(
    [Revenue] - [Revenue Previous Year],
    [Revenue Previous Year]
)
```

---

## Opening the Report

### Requirements

```text
Power BI Desktop
```

### Steps

1. Download the `.pbix` file
2. Open it using Power BI Desktop
3. Refresh the data model if necessary
4. Explore the interactive dashboards

---

## Notes

This report was developed as part of a Business Intelligence portfolio project and uses a fictional training dataset intended exclusively for educational and demonstration purposes.
