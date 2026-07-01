# 🚜 Agricultural Sales Analytics Dashboard

![Portfolio Project](https://img.shields.io/badge/Portfolio-Project-blue?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Analytics-orange?style=for-the-badge)
![Business Intelligence](https://img.shields.io/badge/Business_Intelligence-Reporting-success?style=for-the-badge)
![Data Modeling](https://img.shields.io/badge/Data_Modeling-Star_Schema-purple?style=for-the-badge)

End-to-end Business Intelligence project developed in Power BI to analyze sales performance, customer behavior, product portfolio, regional distribution and revenue trends across multiple years.

The solution leverages dimensional modeling, DAX measures and interactive dashboards to provide actionable insights for commercial management and strategic decision-making.

---

## 🎯 Project Highlights

- Interactive Power BI dashboard
- Star schema data model
- Multi-year sales analysis
- Revenue and profitability monitoring
- Time intelligence calculations
- Regional performance analysis
- Customer segmentation and ranking
- Product portfolio analytics
- KPI monitoring
- Executive reporting

---

## 🚀 Overview

This project analyzes agricultural equipment sales across multiple brands, product categories, customers and geographic regions.

The dashboard enables users to:

- Monitor revenue performance
- Compare yearly results
- Analyze seasonality patterns
- Evaluate product portfolio performance
- Identify top customers
- Monitor regional sales distribution
- Support commercial decision-making

---

## 📷 Dashboard Preview

The report was designed to support executive analysis through a unified sales performance view.

### Main Analysis Areas

#### 1. Revenue Overview & Seasonality

- Revenue evolution by month
- Year-over-year comparison
- Annual revenue performance
- Seasonality patterns

#### 2. Portfolio & Regional Analysis

- Sales distribution by region
- Revenue by sales management area
- Product category performance
- Brand comparison

#### 3. Customer Analytics

- Top customers by revenue
- Bottom customers by purchase volume
- Customer concentration analysis
- Commercial performance monitoring

```text
dashboard/
├── revenue_overview.png
├── regional_performance.png
└── customer_analysis.png
```

---

## 🏗️ Data Model

The solution follows a dimensional modeling approach using a star schema.

```text
                 Calendar
                     │
                     │
Customers ─── Sales Fact ─── Products
                     │
                     │
               Categories
```

### Fact Table

```text
Sales
```

Core metrics:

- Quantity Sold
- Unit Price
- Revenue

### Dimension Tables

```text
Customers
Products
Categories
Calendar
```

---

## 📂 Project Structure

```text
agricultural-sales-analytics-dashboard/
│
├── dashboard/
│   ├── revenue_overview.png
│   ├── regional_performance.png
│   └── customer_analysis.png
│
├── sample_data/
│   ├── customers_sample.csv
│   ├── products_sample.csv
│   ├── categories_sample.csv
│   ├── sales_sample.csv
│   └── calendar_sample.csv
│
├── dax/
│   └── measures.md
│
├── power_bi/
│   └── Agricultural_Sales_Analytics.pbix
│
└── README.md
```

---

## 📊 Business Metrics

The dashboard includes key commercial indicators such as:

### Revenue Metrics

- Total Revenue
- Revenue by Year
- Revenue by Month
- Revenue Growth (%)
- Revenue by Brand

### Customer Metrics

- Top Customers
- Bottom Customers
- Revenue Concentration
- Purchase Volume

### Product Metrics

- Revenue by Product
- Revenue by Category
- Sales Volume by Product
- Product Ranking

### Regional Metrics

- Revenue by State
- Revenue by Sales Region
- Revenue by Sales Management Area

---

## 📈 Analytical Capabilities

### Time Intelligence

The solution supports:

- Year-over-Year (YoY)
- Year-to-Date (YTD)
- Monthly comparisons
- Trend analysis
- Seasonality analysis

---

### Commercial Performance

Users can monitor:

- Sales evolution
- Revenue growth
- Customer purchasing behavior
- Product demand
- Brand performance

---

### Geographic Analysis

Interactive regional analysis includes:

- State-level performance
- Regional comparisons
- Sales management performance
- Revenue concentration analysis

---

## 📊 Sample Data

Representative datasets are included for demonstration purposes.

### Available Datasets

```text
sample_data/
├── customers_sample.csv
├── products_sample.csv
├── categories_sample.csv
├── sales_sample.csv
└── calendar_sample.csv
```

### Data Characteristics

All sample datasets are:

- Anonymized
- Portfolio-friendly
- Structurally equivalent to production datasets
- Free from confidential information
- Suitable for learning and demonstration

---

## 🧮 Sample DAX Measures

Examples of analytical calculations included in the project:

```DAX
Revenue =
SUMX(
    Sales,
    Sales[Quantity Sold] * Sales[Unit Price]
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

Additional measures include:

- Ranking
- Time Intelligence
- Running Totals
- Year-over-Year Comparisons
- Customer Segmentation

---

## 💻 Power BI Features

The report demonstrates several Power BI capabilities:

- Dimensional data modeling
- DAX calculations
- KPI cards
- Interactive filtering
- Geographic visualizations
- Ranking analysis
- Time intelligence
- Drill-down navigation

---

## 🚀 Getting Started

### Requirements

- Power BI Desktop
- Sample datasets (optional)

---

### Open the Project

```text
power_bi/
└── Agricultural_Sales_Analytics.pbix
```

---

### Explore the Data Model

```text
Customers
Products
Categories
Calendar
Sales
```

---

### Interact with the Dashboard

Available slicers include:

- Year
- Brand
- Product Class
- State
- Sales Region

---

## 📈 Business Value

The dashboard provides a centralized commercial analytics environment that supports strategic and operational decisions.

Key benefits include:

- Increased visibility into sales performance
- Improved customer analytics
- Better product portfolio management
- Revenue trend monitoring
- Regional performance tracking
- Faster decision-making
- Enhanced KPI governance

---

## 🧩 Technologies Used

- Power BI
- DAX
- Power Query
- Data Modeling
- Star Schema
- Business Intelligence

---

## 🧠 What This Project Demonstrates

- Business Intelligence development
- Dashboard design
- Data visualization
- Dimensional modeling
- DAX development
- Time intelligence
- KPI monitoring
- Revenue analytics
- Customer analytics
- Product analytics
- Geographic analysis
- Executive reporting

---

## 🔒 Disclaimer

This repository contains a portfolio version of a commercial analytics project.

- No confidential information is included
- Sample datasets are anonymized
- Business data has been adapted for demonstration purposes
- Files are intended exclusively for educational and portfolio use

---

## ⭐ Final Notes

This project showcases the complete development cycle of a Business Intelligence solution, from data modeling and metric definition to dashboard design and executive reporting.

The focus is on delivering scalable, maintainable and business-oriented analytics capable of supporting commercial performance management and strategic decision-making.

---

## 👤 Author

Data Analytics professional specializing in:

- Power BI
- Data Modeling
- DAX
- Business Intelligence
- Data Engineering
- Analytics Engineering

---

## 📬 Contact

Feel free to reach out for questions or discussions about this project.
