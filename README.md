# 📊 Microsoft Power BI Data Analyst — Capstone Project

> Microsoft Excel · Power BI · DAX · Power Query · Python · Power BI Service

An end-to-end business intelligence project completed as the Microsoft
Power BI Data Analyst Professional Certificate Capstone on Coursera.
The project simulates a real-world analytics engagement for Tailwind
Traders — a global retail company — covering the complete Power BI
workflow from raw data preparation through to an executive dashboard
published in Power BI Service.

---

## 📌 Project Objectives

- Prepare and validate sales data in Excel before Power BI integration
- Build a structured data model connecting Sales, Purchases, Countries,
  and Currency Exchange tables
- Write DAX measures for profit margins, time intelligence, and median sales
- Design interactive Sales and Profit Overview report pages
- Publish an executive dashboard with mobile layout in Power BI Service
- Configure data alerts and weekly report subscriptions

---

## 🗂️ What Was Built

**Data Preparation — Excel**
Calculated Gross Revenue, Total Tax, and Net Revenue using Excel
formulas before loading into Power BI.

**Data Transformation — Power Query**
Loaded four data sources, assigned correct data types, filtered
out returned purchases, and ingested currency exchange data via
a Python script using Pandas.

**Data Modeling**
Built relationships between Sales, Purchases, Countries, and
Exchange Data tables. Created a Calendar table and a Sales in USD
calculated table using ADDCOLUMNS and RELATED to convert all
revenue figures into a unified currency.

**DAX Measures**
```dax
Yearly Profit Margin = DIVIDE(SUM([Profit USD]), SUM([Net Revenue USD]))
Quarterly Profit     = CALCULATE(SUM([Profit USD]), DATESQTD(CalendarTable[Date]))
YTD Profit           = TOTALYTD(SUM([Profit USD]), CalendarTable[Date])
Median Sales         = MEDIAN([Gross Revenue USD])
```

**Report Design**
Two-page report covering Sales Overview and Profit Overview —
bar, column, pie, line, area, and donut charts with KPI cards,
slicers, and trend lines.

**Executive Dashboard — Power BI Service**
Pinned visuals from both report pages into a single executive
dashboard with full mobile layout configured for cards, KPIs,
and all core visualizations.

**Subscriptions & Alerts**
Configured a Gross Revenue alert at $400 threshold and weekly
email subscriptions for both Sales and Profit report pages.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data preparation and revenue calculations |
| Power BI Desktop | Data modeling, DAX, and report design |
| Power Query | Data transformation and type assignment |
| DAX | Profit, revenue, and time intelligence measures |
| Python (Pandas) | Currency exchange data ingestion |
| Power BI Service | Dashboard, alerts, and subscriptions |

---

## 📚 Skills Demonstrated

- Full Power BI workflow from raw data to published dashboard
- Power Query transformation across multiple data sources
- Relational data modeling with calculated tables
- DAX — TOTALYTD, DATESQTD, MEDIAN, ADDCOLUMNS, RELATED, DIVIDE
- Multi-page report design with 6+ visual types
- Executive dashboard with mobile layout configuration
- Power BI Service publishing, subscriptions, and data alerts

---

## 👨‍💻 Author

**Kaviraj Desai**
- LinkedIn: [linkedin.com/in/kavirajdesai](https://linkedin.com/in/kavirajdesai)
- GitHub: [github.com/kavirajdesai](https://github.com/kavirajdesai)
