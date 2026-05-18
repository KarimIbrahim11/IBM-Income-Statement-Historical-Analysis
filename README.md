# IBM Financial Performance Dashboard

## Project Overview

This project is a complete Financial Analysis Dashboard developed using IBM annual income statement data extracted from the Alpha Vantage API using Python.

The goal of the project is to transform raw financial statement data into an interactive dashboard capable of providing business insights, profitability analysis, expense analysis, operational efficiency tracking, and executive-level reporting.

The project combines Financial Analysis, Business Intelligence, Data Analytics, and Data Visualization concepts using Excel and Microsoft's BI stack.

---

# Project Objectives

The dashboard was designed to answer key business questions such as:

- Is IBM growing over time?
- How has revenue changed across years?
- Are profit margins improving or declining?
- Which expense categories consume the largest portion of revenue?
- How efficient is the company's operations?
- How do EBITDA and Net Income compare?
- Is the company controlling operating expenses effectively?

---

# Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Python | Data Extraction |
| Requests Library | API Requests |
| Pandas | Data Transformation |
| CSV | Data Storage |
| Excel | Dashboard Development |
| Power Query | Data Cleaning & Transformation |
| Power Pivot | Data Modeling |
| DAX | Financial Measures & KPIs |
| Pivot Tables | Aggregation |
| Pivot Charts | Data Visualization |

---

# Project Workflow

```text
Financial API Extraction
        ↓
Raw CSV Dataset
        ↓
Excel Raw Data Layer
        ↓
Power Query Cleaning & Transformation
        ↓
Power Pivot Data Modeling
        ↓
DAX Measures & KPIs
        ↓
Pivot Tables
        ↓
Pivot Charts
        ↓
Interactive Financial Dashboard
```

---

# Data Collection

The financial data was collected using the Alpha Vantage API.

The dataset contains IBM annual income statement reports including:

- Revenue
- Gross Profit
- Operating Income
- Net Income
- EBITDA
- Operating Expenses
- SG&A
- R&D
- Interest Expense
- Tax Expense
- Other Financial Metrics

---

# Data Extraction Process

Python was used to connect to the Alpha Vantage API and extract IBM annual financial reports.

The extracted JSON response was converted into a Pandas DataFrame and exported as a CSV file for further analysis in Excel.

---

# Data Cleaning & Transformation

Power Query was used to clean and prepare the dataset before analysis.

## Cleaning Steps

- Removed unnecessary columns
- Converted data types
- Converted date fields
- Renamed columns
- Structured the dataset for analysis
- Prepared the data model for Power Pivot

---

# Data Modeling

The project follows a layered BI architecture:

```text
Raw Data Layer
    ↓
Transformation Layer
    ↓
Semantic Layer
    ↓
Visualization Layer
```

---

# Raw Data Layer

The raw financial dataset was stored in a dedicated Excel sheet without modifications.

This layer acts as the main data source for the project.

---

# Power Pivot Data Model

Power Pivot was used to create a semantic financial model.

The model includes:

- Financial table
- DAX Measures
- Financial KPIs

---

# Financial KPIs

Several important financial KPIs were created using DAX:

| KPI |
|---|
| Total Revenue |
| Revenue Growth % |
| Gross Margin |
| Operating Margin |
| Net Margin |
| EBITDA Margin |
| Expense Ratio |
| SG&A Ratio |
| R&D Ratio |
| Tax Rate |
| Interest Coverage Ratio |

---

# Dashboard Development

Pivot Tables and Pivot Charts were used to build the dashboard visuals.

The dashboard includes multiple financial analysis sections.

---

# Dashboard Sections

## KPI Cards

Executive-level KPI cards showing:

- Total Revenue
- Gross Margin
- EBITDA Margin
- Net Margin
- Revenue CAGR
- Average Revenue Growth

---

## Revenue Analysis

Visualizations used to analyze company growth trends over time.

---

## Profitability Analysis

Analysis of company profitability performance.

---

## Expense Analysis

Analysis of operating expenses and expense structure.

---

## Operational Efficiency Analysis

Analysis of business operational performance and cost efficiency.

---

## Tax & Interest Analysis

Analysis of tax burden and interest expense impact on profitability.

---

# Dashboard Features

The dashboard includes:

- Interactive Pivot Charts
- Dynamic filtering
- Year-based analysis
- Financial KPI tracking
- Expense composition analysis
- Profitability trend analysis
- Executive-level reporting visuals

---

# Financial Analysis Performed

The project includes several types of financial analysis:

- Revenue Growth Analysis
- Margin Analysis
- Profitability Analysis
- Expense Analysis
- Operational Efficiency Analysis
- Trend Analysis
- Year-over-Year Analysis
- Financial KPI Monitoring

---

# Business Insights Generated

The dashboard helps identify:

- Revenue growth trends
- Profitability performance
- Expense structure changes
- Cost efficiency trends
- EBITDA performance
- Tax and interest impact
- Financial performance fluctuations

---

# Skills Demonstrated

This project demonstrates skills in:

- Financial Analysis
- Data Analytics
- Business Intelligence
- Dashboard Design
- Data Visualization
- DAX
- Power Pivot
- Power Query
- Python Data Extraction
- API Integration
- Executive Reporting

---


# Conclusion

This project demonstrates how raw financial statement data can be transformed into an interactive executive-level financial dashboard using Python, Excel, Power Query, Power Pivot, DAX, Pivot Tables, and Pivot Charts.

The dashboard provides valuable business insights into IBM's financial performance, profitability, expense management, and operational efficiency over time.
