# Data Extraction Guide

This document explains the Python code used to extract IBM financial statement data from the Alpha Vantage API and prepare it for financial analysis and dashboard development.

---

# Python Data Extraction Code with Step-by-Step Explanation

```python
import requests
# Imports the requests library used to send HTTP requests to APIs.

url = "https://www.alphavantage.co/query"
# Stores the Alpha Vantage API endpoint URL.

params = {
    "function": "INCOME_STATEMENT",
    # Specifies that we want income statement financial data.

    "symbol": "IBM",
    # Specifies the company ticker symbol (IBM).

    "apikey": "YOUR_API_KEY"
    # API authentication key required to access Alpha Vantage data.
}

response = requests.get(url, params=params)
# Sends a GET request to the API endpoint with the specified parameters.

response.raise_for_status()
# Checks if the request was successful.
# Raises an error if the API request fails.

data = response.json()
# Converts the API response from JSON format into a Python dictionary.

data.keys()
# Displays the top-level keys available in the JSON response.
# Useful for exploring the API structure.

import pandas as pd
# Imports the pandas library used for data manipulation and analysis.

annual_df = pd.DataFrame(data["annualReports"])
# Converts the annual income statement reports into a pandas DataFrame.

annual_df
# Displays the DataFrame containing IBM annual financial statement data.

annual_df.to_csv(
    r'C:\Users\hb\OneDrive\Desktop\Income statment\Income statment.csv'
)
# Exports the DataFrame to a CSV file for further analysis in Excel.
```

---

# API Response Structure

The API returns financial statement data in JSON format.

Example structure:

```text
{
    "symbol": "IBM",
    "annualReports": [...],
    "quarterlyReports": [...]
}
```

---

# Key Components Explained

| Component | Purpose |
|---|---|
| requests | Sends HTTP requests to APIs |
| params | Stores API query parameters |
| response | Contains API response data |
| response.json() | Converts JSON response into Python dictionary |
| pandas DataFrame | Converts structured data into tabular format |
| to_csv() | Saves data locally as CSV |

---

# Why This Approach Was Used

This extraction workflow provides several advantages:

- Automated financial data collection
- Scalable API-based workflow
- Structured tabular dataset creation
- Easy integration with Excel and BI tools
- Reusable financial data pipeline

---

# Output Dataset

The generated CSV file contains IBM annual income statement data including:

- Revenue
- Gross Profit
- Operating Income
- Net Income
- EBITDA
- Operating Expenses
- SG&A
- Research & Development
- Interest Expense
- Tax Expense
- Other financial metrics

---

# Next Steps After Extraction

After extracting the data:

1. Import CSV into Excel
2. Clean and transform data using Power Query
3. Build a Power Pivot data model
4. Create DAX measures
5. Build Pivot Tables and Pivot Charts
6. Develop the Financial Dashboard

---

# Workflow Summary

```text
Alpha Vantage API
        ↓
Python Requests
        ↓
JSON Response
        ↓
Pandas DataFrame
        ↓
CSV Export
        ↓
Excel Analysis
        ↓
Power Query
        ↓
Power Pivot
        ↓
DAX Measures
        ↓
Financial Dashboard
```
