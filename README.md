# Austin-Bank-Data-Quality-Exploratory-Data-Analysis

## Problem Statement

Banks often face challenges in leveraging operational data due to quality issues such as missing values, inconsistent formats, and erroneous entries. These issues hinder the ability to generate accurate insights for performance monitoring and strategic planning. This project addresses these challenges by analyzing a banking dataset to identify and resolve data quality problems while uncovering trends in customer volume and deposit patterns across cities, service categories, and time periods. The goal is to transform raw data into a clean, analysis-ready format and generate actionable insights to support data-driven decisions, optimize banking operations, and improve service delivery.

---

## Tools Used

- Python: pandas, numpy, matplotlib, seaborn
- Jupyter Notebook

---

## Process Breakdown

### Data Quality Issues & Cleaning

- Missing Values: Imputed 3 missing values in `Customer Volume/Deposit Value` using median imputation.
- Negative Values: Replaced 3 negative numeric values with median after converting them to NaN.
- Inconsistent Dates: Corrected invalid years (2073 → 2023) and standardized date formats.
- Duplicates: Verified zero duplicate entries.
- Categorical Standardization:
  - Example: `Bond%%%% savings → Bonds savings accounts`
  - Example: `Cardi££££££ → Cardiff`

---

### Feature Engineering

- Created new fields: `Date` (datetime), `Quarter`, `Year/Month` for time-based analysis.

---

## Data Analysis & Visualization

### Monthly Trends

- Aggregated total Customer Volume and Deposit Value by Month-Year.
- Table 1: Monthly trends overview.

### City Benchmarks

- Compared quarterly averages for cities: Oxford, Edinburgh, Cardiff.
- Table 2: City-wise performance metrics.

### Service Category Performance

- Evaluated quarterly performance across services like Current accounts, Bonds savings, etc.
- Table 3: Category-wise trends and benchmarks.

---

## EDA Summary

| Metric               | Value                                 |
|----------------------|----------------------------------------|
| Top-Performing       | Current accounts (avg. deposit: £668K) |
| Lowest Volume        | Children’s savings (avg. volume: 37.8K)|
| Best City Performance| Oxford (peaked £7.77M in Q3 2023)      |
| Category Contribution| Current accounts: 56% of total deposits (£72.1M) |

---

## Impact & Insights

- Resolved over 15% of data entry errors, enabling reliable trend analysis.
- Developed quarterly dashboards to support data-driven planning.
- Identified high-performing areas to scale (Current accounts) and low performers to optimize (Children’s savings).

---

## Outcome

This project delivers:
- A cleaned, structured dataset ready for strategic planning.
- Modular Python functions for handling missing and negative values.
- GroupBy aggregation pipelines for benchmarking.
- Seaborn visualizations setup (charts executable in Jupyter Notebook).

---

## Key Highlights

- Data Quality: Automated correction of dates, negatives, and label inconsistencies.
- Benchmarking: Comparative analysis using `groupby()` and `.agg()`.
- Scalability: Modular functions for data wrangling and preparation.
- Visualization Ready: Configured Seaborn charts for trends and patterns.

---

## Folder Structure (Suggested)

