# Austin-Bank-Data-Quality-Exploratory-Data-Analysis

## Overview

This project analyzes a banking dataset to identify data quality issues and extract actionable insights into customer volume and deposit trends across cities, service categories, and time periods. The objective is to support data-driven decision-making for optimizing banking operations and enhancing service offerings.

---

## Table of Contents

- [Problem Statement](#problem-statement)
- [Tools and Technologies](#tools-and-technologies)
- [Process Breakdown](#process-breakdown)
  - [Data Cleaning](#data-cleaning)
  - [Feature Engineering](#feature-engineering)
  - [Data Analysis and Visualization](#data-analysis-and-visualization)
- [Key Findings](#key-findings)
- [Business Impact](#business-impact)
- [Outcome](#outcome)
- [Highlights](#highlights)

---

## Problem Statement

Analyze a banking dataset to:

- Identify and correct data quality issues.
- Uncover trends in customer volume and deposit value by city, service category, and time period.
- Enable strategic, data-driven decisions for bank operations and service development.

---

## Tools and Technologies

- **Language**: Python
- **Libraries**:
  - pandas, numpy – data manipulation and cleaning
  - matplotlib, seaborn – data visualization
- **Environment**: Jupyter Notebook

---

## Process Breakdown

### Data Cleaning

- **Missing Values**:  
  Imputed 3 missing values in `Customer Volume` and `Deposit Value` using median.

- **Negative Values**:  
  Replaced 3 negative numeric entries with column median after converting to NaN.

- **Date Inconsistencies**:  
  Corrected invalid year `2073` to `2023` and standardized all date formats.

- **Duplicate Records**:  
  Verified dataset contained no duplicate entries.

- **Categorical Standardization**:
  - `Bond%%%% savings` → `Bonds savings accounts`
  - `Cardi££££££` → `Cardiff`

---

### Feature Engineering

Created new time-based features:

- `Date` – parsed from original fields
- `Quarter`
- `Year/Month`

---

### Data Analysis and Visualization

- **Monthly Trends**:
  - Aggregated total customer volume and deposit value by month-year (Table 1).

- **City Benchmarks**:
  - Quarterly average customer/deposit trends across Oxford, Edinburgh, and Cardiff (Table 2).

- **Service Category Performance**:
  - Quarterly performance for service types like `Current accounts` and `Bonds savings accounts` (Table 3).

---

## Key Findings

- **Top-performing category**:  
  `Current accounts` with an average deposit of **£668K**.

- **Lowest customer volume**:  
  `Children’s savings` with an average of **37.8K** customers.

---

## Business Impact

- **Oxford** dominated deposits, peaking at **£7.77M in Q3 2023**.

- **Current accounts** contributed to **56% of total deposits (£72.1M)**.

- **15%+ of records** corrected through data cleaning, ensuring reliable analysis.

- **Quarterly dashboards** developed to guide regional resource allocation and product strategy.

---

## Outcome

The project delivers a clean and analysis-ready dataset supported by:

- Modular data cleaning and transformation pipeline.
- Exploratory data analysis for performance tracking.
- Insightful summaries to assist with service scaling and operational decisions.

---

## Highlights

- **Automated Data Cleaning**:  
  Standardized inconsistent entries, handled missing and negative values.

- **Comparative Benchmarking**:  
  Leveraged `groupby()` and `agg()` for city and service performance comparisons.

- **Reusable Code**:  
  Modular functions for scalability across similar datasets.

- **Visualization-Ready**:  
  Charts prepared with seaborn for trend analysis (visuals excluded from README).

---

## License

This project is for academic and educational purposes. Licensing terms to be added based on usage.

---

## Contact

For feedback or collaboration, please reach out via GitHub or email.

