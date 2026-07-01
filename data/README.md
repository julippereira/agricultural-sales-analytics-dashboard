# 📊 Data

This directory contains the datasets used to build the Agricultural Sales Analytics Dashboard.

The data represents a fictional commercial operation and was originally created for educational and training purposes.

---

## Available Datasets

```text
data/
├── customers.csv
├── products.csv
├── categories.csv
├── sales.csv
└── calendar.csv
```

---

## Dataset Description

### customers.csv

Customer master data.

Main fields:

- Customer ID
- Company Name
- State (UF)
- Sales Region
- Sales Management Area

---

### products.csv

Product catalog.

Main fields:

- Product ID
- Product Name
- Brand
- Product Class
- Category ID
- Category Description

---

### categories.csv

Product category hierarchy.

Main fields:

- Category ID
- Category
- Product Class

---

### sales.csv

Transactional sales records.

Main fields:

- Product ID
- Customer ID
- Sales Date
- Quantity Sold
- Unit Price

---

### calendar.csv

Date dimension table used for time intelligence calculations.

Main fields:

- Date
- Month
- Month Name
- Year
- Semester
- Day Attributes

---

## Data Model

```text
                 calendar
                     │
                     │
customers ─── sales ─── products
                     │
                     │
                categories
```

---

## Usage

The datasets can be imported directly into:

- Power BI
- Excel
- Python (Pandas)
- SQL databases
- Other BI and analytics tools

---

## Disclaimer

These datasets are provided exclusively for educational and portfolio purposes.

- No real customer information is included
- No confidential business information is included
- Data has been prepared for demonstration and learning scenarios
