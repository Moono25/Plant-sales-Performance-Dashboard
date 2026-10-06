# Plant.Co Sales Performance Perport Dashboard
> This is a performance dashboard that compares the prior year to the current years sales and gross profit percentage the current year stacks up against the present.Those metrics will be checked against sales, quantity and gross profit. This provides a clear way to compare previous performace vs current.

---

## ⚙️ Project Type Flags
> *Check what applies. This helps reviewers and collaborators understand the nature of the work at a glance. Delete this block before publishing.*

- [ ] Exploratory Data Analysis (EDA)
- [ ] Dashboard / Data Visualization
- [ ] Data Pipeline / ETL
- [ ] Predictive Modelling / Machine Learning
- [ ] Data Cleaning / Wrangling
- [ ] DAX

---

## Table of Contents
1. [Project Overview](#1-project-overview)
2. [Objectives](#2-objectives)
3. [Project Scope & Tools](#3-project-scope--tools)
4. [Repository Structure](#4-repository-structure)
5. [Data Workflow](#5-data-workflow)
6. [Data Model & Schema](#6-data-model--schema)
7. [Analysis & Metrics](#8-analysis--metrics)
8. [Key Insights](#9-key-insights)
9. [Recommendations](#10-recommendations)
10. [Assumptions & Limitations](#11-assumptions--limitations)
11. [Future Enhancements](#12-future-enhancements)
12. [Deliverables](#13-deliverables)
13. [Author](#14-author)

---

## 1. Project Overview

<!--
  
-->

**Context:** [This project looks at the profiability of an international plant company that cells indoor, outdoor and landscaping plants  spanning across two years]

**Problem Statement:** [This is 
    meant to check whether the comapny is a going conern as in profitable, by comparing the current year to the previous year as way to measure sales and  profitability, this provides an easy effcient way of tracking the stores performance.]

**Approach:** [The performance report shows the bottom ten countries, their performance in sales each month, product actegory and  looking at profitability accross different accounts.]

**Outcome:** [Profitablity declined bythe final year an accounts reduced explaining the  an there was a steady decline in performance from 2023 t0 2024.?]

---

## 2. Objectives


- **Primary Objective:** [Build a Power BI dashboard that compares the current year against the previous one]
- **Secondary Objective 1:** [To quantitfy changes in sales, gross profit, quantity and gross profit percentage of current and previous years]
- **Secondary Objective 2:** [Find any differences in sales across dimensions like country, product type, and accounts]


---

## 3. Project Scope & Tools

### Scope

| Dimension | Details |
|-----------|---------|
| **In Scope** | Plant.Co's Product and Accounts data across the world, Jan 2022 to April 2024. 
    The analysis covers Product type, country, gross profit, gross profit percentage, year-to-date prior, year-to-date and year-to-date vs prior year-to-date. |
| **Out of Scope**| The sizes of the products, the individual customers that made purchases.
    The reason product sizes were removed was that they do not affect sales in this case; customer information is not needed to perform this report.|
| **Time Period** | This data contains information from three years, 2022 to 2024. |
| **Granularity** | This analysis moves from years down to quarters, then months. |

### Tools & Technologies

| Category | Tool(s) Used |
|----------|-------------|
| Data Source | [Plant_DTS.xls] |
| Data Preperation | [Power Query / PowerBI data transformation] |
| Data Modeling | [Power BI relationships, dimensional model] |
| Analysis | [DAX measures] |
| Visualization | [Power BI] |
| Documentation | [Markdown/ GitHub] |

---

## 4. Repository Structure

```
[project-root]/
│
├── data/
│   ├── Plant_DTS.xls         # Original, unmodified source data - never edited
│
├── reports/
│   ├── Project_Performance_report.pbix
│
├── visuals/
│   ├── screenshots   # Exported charts, dashboard screenshots, ERD diagrams
│
├── docs/
│   ├── data_dictionary.md  # Data dictionaries, schema notes, reference material
│
├── project_metadata.yml      # Machine-readable metadata (optional)
└── README.md                 # You are here


## 5. Data Workflow
Plant_DTS
      ↓
PowerBI- Power Query
      ↓
Data cleaning & Transformation
      ↓
Data modeling and relationships
      ↓
Dax Measures
      ↓
Interactive Dashboards
```

1. **Source:** The project uses the Plant_DTS.xls dataset as the source of the sales and related business data.
2. **Ingestion:** The source workbook was imported into Power BI for preparation and analysis.
3. **Cleaning:** The source data was reviewed and prepared using Power Query to ensure that the tables and fields were suitable for analysis.
4. **Data Modeling:** Relationships were established between the relevant tables within the Power BI data model.
5. **Transformation:** Data was transformed into a structure suitable for the dashboard and analytical calculations by removing empty columns and making sure formats were consistent.
6. **Analysis:** DAX measures were created to calculate sales-performance metrics including YTD, PYTD, YTD vs PYTD, quantity, gross profit and gross profit percentage.
7. **Output:** The prepared data and measures were presented through an interactive Power BI sales performance dashboard.

---

## 6. Data Model & Schema


### Dataset / Table: `Plant_FACT`

| Field / Attribute | Purpose |
|-------------------|---------|
| Sales information | Used to calculate sales performance |
| Quantity | Used to evaluate sales volume |
| Gross Profit | Used to evaluate profitability |
| Date | Used for time-based analysis |
| Account | Used to analyse performance across accounts |
| Product information | Used to analyse performance by product type |
| Country | Used for geographic analysis |

> ### Accounts

The `Accounts` table contains account-level information used to analyse sales performance across different accounts.

### Plant_Hierarchy

The `Plant_Hierarchy` table contains product hierarchy information used to categorise and analyse products.

### Relationships

The tables are connected within the Power BI data model so that sales measures from the `Plant_FACT` table can be analysed using account and product attributes.


## 7. Analysis & Metrics

### Analytical Approach

The analysis uses comparative sales-performance analysis to evaluate current-period performance against the previous period. The dashboard combines time-based analysis with breakdowns by country, product type and account to identify changes in sales volume and profitability.

### Key Metrics Defined

| Metric | Plain-Language Definition | Why It Matters |
|--------|--------------------------|----------------|
| **Sales** | Total sales value generated during the selected period. | Measures overall revenue performance. |
| **Quantity** | Total quantity of products sold during the selected period. | Measures sales volume independently of sales value. |
| **Gross Profit** | Profit generated after accounting for the relevant cost of sales. | Measures the profitability generated from sales. |
| **Gross Profit %** | Gross profit expressed as a percentage of sales. | Shows profitability relative to sales value. |
| **YTD** | Sales or performance accumulated from the beginning of the selected year to the selected date. | Shows current-year performance to date. |
| **PYTD** | The equivalent year-to-date period from the previous year. | Provides a comparable baseline for current performance. |
| **YTD vs PYTD** | Comparison between current YTD performance and the corresponding previous-year period. | Identifies whether performance has improved or declined. |

### Methods Used

- Year-to-date and previous-year-to-date comparison
- Time-based trend analysis
- Geographic performance analysis
- Product-type performance analysis
- Account-level performance analysis
- Comparative analysis of sales, quantity and profitability

---

## 8. Key Insights
**Insight 1: [Sales performance changed across the comparison period]**  
The dashboard allows current-period sales performance to be compared with the corresponding previous period, highlighting changes in overall sales performance.

**Insight 2: [Sales volume and profitability do not necessarily move together]**  
Comparing quantity, sales and gross profit provides a broader view of performance than relying on sales value alone.

**Insight 3: [Performance varies across business dimensions]**  
The dashboard shows differences in performance across countries, product types and accounts, allowing areas of stronger and weaker performance to be identified.

**Insight 4: [Profitability requires separate monitoring]** 

Gross profit and gross profit percentage provide additional context when evaluating sales performance and help distinguish revenue growth from changes in profitability.

---

## 9. Recommendations
---

| Priority | Recommendation | Based On | Suggested Owner |
|----------|---------------|----------|-----------------|
| High | Investigate countries and accounts showing sustained weaker sales or profitability performance to identify the factors contributing to the decline. | Geographic and account-level performance analysis | Sales / Management |
| High | Monitor gross profit percentage alongside sales when evaluating performance so that increases in sales volume are considered alongside profitability. | Sales and profitability comparison | Management / Finance |
| Medium | Review product-type performance to identify categories contributing most strongly to sales and profitability and those requiring attention. | Product-type analysis | Sales / Product Management |

---

## 10. Assumptions & Limitations
### Assumptions

- The source data was assumed to be representative of the sales activity covered by the dataset.
- The YTD and PYTD calculations are treated as appropriate comparable periods for evaluating performance.
- The definitions of sales, quantity, gross profit and gross profit percentage are based on the definitions provided within the source project/data model.

### Limitations

- The analysis is based on the available Plant.Co dataset and therefore reflects only the information contained in that dataset.
- The dashboard identifies patterns and differences in performance but does not establish the underlying causes of those changes.
- Customer-level purchasing behaviour was outside the scope of the analysis.
- Product size information was excluded from the analysis.
- The project is a follow-along implementation based on an existing Plant.Co dashboard/case study rather than an independent analysis conducted for Plant.Co.
---

## 11. Future Enhancements
---

- [ ] Add more detailed customer-level analysis if suitable customer data becomes available.
- [ ] Expand the dashboard with additional profitability and product-performance analysis.
- [ ] Introduce automated data refresh if the project were connected to a recurring operational data source.
- [ ] Add more detailed drill-through analysis for underperforming countries, products and accounts.

---

## 12. Deliverables

| Deliverable | Description | Location |
|-------------|-------------|----------|
| [Power BI dashboard] | [Interactive Plant.Co performance report dashboard containing the analysis and visualizations.]| [powerbi/PlantCo_Sales_Performance.pbix] |
| [Source dataset]  | [Original Plant.Co dataset used as the source for the analysis.] |  [`/data/Plant_DTS.xls`] |
| [Data dictionary] | [Documentation describing the relevant dataset fields and structure.] | [`/docs/data_dictionary.md`] |
| [Project Documentation] | [README documenting the project, workflow, analysis and findings.] | [`/README.md`] |

---

## 13. Author

**[Mapenzi Moono]**
[Data support/Intern - Data Analyst/ Research Associate/ M&E Assistant]

- 🔗 [https://www.linkedin.com/in/mapenzi-moono-445aaa26a/]
- 💼 [Portfolio or GitHub profile URL]
- 📧 [mapenzimoono345@gmail.com]

---

*Last updated: [Month YYYY]*
*If this template helped you, consider starring the repository.*
