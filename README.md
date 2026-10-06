# Plant.Co Sales Performance Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-blue)
![DAX](https://img.shields.io/badge/DAX-Measures-orange)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-Portfolio-green)

## Project Overview

The **Plant.Co Sales Performance Dashboard** is a Power BI sales analysis project focused on evaluating sales and profitability performance across countries, product types, and accounts.

The analysis compares **Year-to-Date (YTD)** performance with the corresponding **Previous Year-to-Date (PYTD)** period to identify changes in sales, quantity sold, gross profit, and gross profit margin.

The dashboard was developed using a Plant.Co sales dataset covering the period from **January 2022 to April 2024**.

The project demonstrates the use of **Power Query, data modelling, DAX, and interactive Power BI visualisation** to transform raw sales data into a business performance report.

> **Attribution:** This project is a follow-along implementation based on an existing Plant.Co sales performance dashboard/case study. It was completed as a learning project to practise Power BI data preparation, modelling, DAX, and dashboard development. The analysis and documentation in this repository have been organised for portfolio purposes.

---

## Business Problem

Plant.Co needs to understand how its sales and profitability are changing over time and where performance is strongest or weakest.

The dashboard addresses questions such as:

- How are current sales performing compared with the previous year?
- How has gross profit changed?
- Has the quantity of products sold increased or decreased?
- Which countries are contributing the least to sales performance?
- How does performance vary across product types?
- Which accounts are contributing to overall performance?
- Are changes in sales being accompanied by changes in profitability?

---

## Objectives

### Primary Objective

Build an interactive Power BI dashboard that compares current-year performance with the previous-year period.

### Secondary Objectives

1. Quantify changes in:
   - Sales
   - Gross Profit
   - Quantity
   - Gross Profit %
2. Analyse differences in sales performance across:
   - Countries
   - Product types
   - Accounts
3. Present the results through an interactive business performance dashboard.

---

## Project Scope

### Included

- Plant.Co sales data
- January 2022 – April 2024
- Country-level performance
- Product-type performance
- Account-level performance
- Sales
- Quantity
- Gross Profit
- Gross Profit %
- YTD performance
- PYTD performance
- YTD vs PYTD comparisons
- Monthly and quarterly performance trends

### Out of Scope

- Individual customer-level analysis
- Product-size analysis
- Customer-level profitability analysis beyond the account information provided in the dataset

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Power BI** | Dashboard development and visualisation |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Calculated measures and performance metrics |
| **Excel** | Source data |
| **GitHub** | Project documentation and portfolio presentation |
| **Markdown** | Project documentation |

---

## Data Workflow

```text
Raw Plant.Co Data
       ↓
Power Query
       ↓
Data Cleaning & Transformation
       ↓
Data Modelling & Relationships
       ↓
DAX Measures
       ↓
Power BI Visualisations
       ↓
Sales Performance Dashboard
```

The workflow begins with the Plant.Co source data, which is prepared and transformed using Power Query.

The cleaned data is then structured into a relational data model within Power BI. Relationships between the relevant tables allow sales information to be analysed across different dimensions such as products, accounts, and organisational hierarchy.

DAX measures are then used to calculate performance indicators such as YTD, PYTD, and the variance between current and previous-year performance.

The resulting measures are presented through interactive Power BI visuals.

---

## Key Metrics

The dashboard focuses on the following performance indicators:

- **Sales**
- **Quantity**
- **Gross Profit**
- **Gross Profit %**
- **YTD**
- **PYTD**
- **YTD vs PYTD**

These metrics allow the dashboard to evaluate both sales volume and profitability rather than relying on sales alone.

---

## Dashboard

The final Power BI report provides an interactive view of Plant.Co's sales performance.

### Performance Overview

![Plant.Co Performance Dashboard](visuals/screenshots/performa.png)


The dashboard enables users to explore performance across different dimensions, including time, country, product type, and accounts.

> **Note:** Dashboard screenshots are included for portfolio viewing. The `.pbix` file contains the interactive Power BI report.

---

## Key Insights

The analysis is designed to identify:

- Changes in sales performance between periods
- Changes in gross profit and profitability
- Differences between current and previous-year performance
- Countries with comparatively weaker sales performance
- Product categories contributing to sales and profitability
- Accounts contributing to overall performance
- Areas where declining sales or profitability may require further investigation

Specific numerical findings are documented based on the final dashboard results.

---

## Recommendations

Based on the analysis, potential business actions include:

1. **Investigate underperforming countries** to understand the factors contributing to weaker sales.
2. **Review product-type performance** to identify products with stronger sales and profitability.
3. **Examine account-level performance** to determine where sales relationships may require attention.
4. **Monitor profitability alongside sales**, since higher sales do not necessarily translate into higher gross profit.
5. **Track YTD versus PYTD performance regularly** to identify emerging changes before they become larger performance issues.

These recommendations should be interpreted as analytical suggestions rather than operational decisions, since the dataset does not provide all of the contextual information required to determine the underlying causes of performance changes.

---

## Assumptions & Limitations

- The analysis is based on the Plant.Co dataset provided for the project.
- The dataset covers January 2022 to April 2024.
- The analysis reflects the fields and dimensions available in the source data.
- The dashboard identifies performance differences but does not establish the causes of those differences.
- No external market, economic, competitor, or customer research was incorporated.
- The project should therefore be viewed as a **sales performance analysis**, rather than a complete assessment of Plant.Co's overall business health.

---

## Future Enhancements

Possible improvements to the analysis include:

- Adding customer-level analysis where appropriate data is available.
- Incorporating additional profitability measures.
- Adding forecasting to estimate future sales performance.
- Including external factors such as market or regional information.
- Expanding the dashboard with more advanced DAX analysis.
- Automating the refresh process for regularly updated reporting.

---

## Repository Structure

```text
PlantCo-Sales-Performance-Dashboard/
│
├── data/
│   └── Plant_DTS.xls
│
├── docs/
│   └── data_dictionary.md
│
├── powerbi/
│   └── PlantCo_Sales_Performance.pbix
│
├── visuals/
│   └── screenshots/
│
├── .gitignore
└── README.md
```

---

## Deliverables

- **Power BI Dashboard** — Interactive sales performance report
- **Power BI Project File** — `.pbix`
- **Source Dataset** — Plant.Co sales data
- **Dashboard Screenshots** — Static portfolio previews
- **Data Dictionary** — Description of relevant data fields
- **Project Documentation** — Methodology, analysis, insights, and limitations

---

## Author

**Saul Moono**

Data Analytics Portfolio

Skills demonstrated in this project:

**Power BI • Power Query • DAX • Data Modelling • Data Visualisation • Business Analysis**

---

## Project Status

**Completed — Portfolio Project**

This project represents a practical Power BI learning exercise focused on transforming sales data into an interactive business performance dashboard.
