# Methodology

This document explains the complete methodology used to build the IBM Financial Performance Dashboard project, including data extraction, cleaning, modeling, KPI development, and dashboard visualization.

---

# 1. Project Objective

The objective of this project was to transform raw financial statement data into an interactive financial dashboard capable of providing executive-level business insights regarding:

- Revenue growth
- Profitability
- Expense structure
- Operational efficiency
- Financial performance trends
- Strategic business transformation

The project combines Financial Analysis, Data Analytics, and Business Intelligence methodologies.

---

# 2. Data Source

The dataset was collected from the Alpha Vantage Financial Statements API.

## Company Analyzed

- IBM

## Dataset Type

- Annual Income Statement Reports

## Data Source Type

- API-based financial data

---

# 3. Data Extraction Methodology

Python was used to automate the extraction of financial statement data from the Alpha Vantage API.

The extraction process included:

1. Sending API requests using the Requests library
2. Receiving JSON financial data
3. Converting JSON data into tabular format using Pandas
4. Exporting the final dataset into CSV format

---

# 4. Data Storage Layer

The extracted dataset was stored as a CSV file before importing it into Excel.

This layer acts as the raw data source for the entire dashboard workflow.

---

# 5. Data Cleaning & Transformation

Power Query was used for data preparation and transformation.

## Cleaning Steps Performed

- Removed unnecessary columns
- Converted text values into numeric data types
- Converted date columns into proper date formats
- Renamed columns for readability
- Structured the dataset for financial analysis
- Validated missing and null values

---

# 6. Data Modeling Methodology

The project follows a layered Business Intelligence architecture.

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

# 7. Semantic Modeling using Power Pivot

Power Pivot was used to build the financial data model.

The semantic layer included:

- Financial fact table
- Calendar table
- Relationships
- Financial measures
- KPI calculations

This approach improves scalability, reusability, and dashboard performance.

---

# 8. DAX Methodology

DAX (Data Analysis Expressions) was used to create dynamic financial calculations and KPI measures.

## Key DAX Calculations

- Revenue Growth %
- Gross Margin
- Operating Margin
- EBITDA Margin
- Net Margin
- Expense Ratios
- Interest Coverage Ratio
- Year-over-Year Analysis

---

# 9. Time Intelligence Methodology

Time intelligence functions were implemented to analyze financial trends over time.

Functions used include:

- SAMEPERIODLASTYEAR()
- CALCULATE()
- DIVIDE()

These functions enabled:

- Year-over-Year comparisons
- Trend analysis
- Historical performance evaluation

---

# 10. Dashboard Design Methodology

The dashboard was designed using Pivot Tables and Pivot Charts inside Excel.

The design philosophy focused on:

- Executive-level reporting
- Clean financial storytelling
- Interactive analysis
- Business-focused insights
- Visual clarity

---

# 11. Dashboard Structure

The dashboard was divided into multiple analytical sections.

## Sections Included

### KPI Section
Displays high-level financial performance indicators.

### Revenue Analysis
Analyzes revenue trends and growth performance.

### Profitability Analysis
Evaluates margins and profit generation capability.

### Expense Analysis
Analyzes operational cost structure and expense composition.

### Operational Efficiency Analysis
Measures cost control and operational scalability.

### Tax & Interest Analysis
Evaluates non-operating financial impacts.

---

# 12. Financial Analysis Methodology

Several financial analysis techniques were applied throughout the project.

## Analysis Types

- Trend Analysis
- Margin Analysis
- Profitability Analysis
- Expense Structure Analysis
- Efficiency Analysis
- Growth Analysis
- Comparative Analysis
- Year-over-Year Analysis

---

# 13. Visualization Methodology

Different chart types were selected based on business questions and analytical objectives.

## Visualization Types Used

| Visualization | Purpose |
|---|---|
| Line Charts | Trend Analysis |
| Column Charts | Growth Comparison |
| Combo Charts | EBITDA vs Net Income |
| Donut Charts | Expense Composition |
| Stacked Area Charts | Expense Trends |
| KPI Cards | Executive Summary Metrics |

---

# 14. Business Intelligence Approach

The project was built using a BI-oriented workflow rather than a simple spreadsheet analysis approach.

The workflow emphasized:

- Data layering
- Semantic modeling
- Reusable measures
- Dynamic KPIs
- Interactive analysis
- Financial storytelling

---

# 15. Forecasting Methodology

Forecast values were generated using historical trend analysis within Excel.

The forecasting section was designed to estimate future revenue and profitability trends based on historical performance patterns.

Forecast figures should be considered directional estimates rather than official financial guidance.

---

# 16. Key Business Questions Answered

The dashboard was designed to answer several important business questions:

- Is IBM growing over time?
- Are profitability margins improving?
- Which expenses consume the largest share of revenue?
- Is operational efficiency improving?
- How resilient is profitability during contraction periods?
- How do EBITDA and Net Income trends compare?

---

# 17. Project Architecture

```text
Alpha Vantage API
        ↓
Python Extraction
        ↓
CSV Storage
        ↓
Excel Raw Data
        ↓
Power Query Cleaning
        ↓
Power Pivot Modeling
        ↓
DAX Measures
        ↓
Pivot Tables
        ↓
Pivot Charts
        ↓
Financial Dashboard
        ↓
Business Insights
```

---

# 18. Project Outcome

The final result is an executive-level financial dashboard capable of delivering:

- Financial performance monitoring
- Strategic business insights
- Profitability analysis
- Expense analysis
- Operational efficiency evaluation
- Trend visualization
- Executive reporting

The project demonstrates how raw financial statement data can be transformed into a scalable Business Intelligence solution using Python, Excel, Power Query, Power Pivot, and DAX.
