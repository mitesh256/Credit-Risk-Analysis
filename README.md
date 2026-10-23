# Credit Risk Analysis Dashboard | Power BI

An interactive Power BI dashboard for analyzing loan portfolio performance, credit risk distribution, repayment status, and default patterns.

## 📌 Project Overview

The Credit Risk Analysis Dashboard is a data analytics project developed using Microsoft Power BI. It explores loan portfolio data to understand risk distribution, default behavior, outstanding loan exposure, and lending trends.

The dashboard combines key performance indicators (KPIs), interactive visualizations, and slicers to help users examine loan performance across risk categories, employment statuses, loan purposes, credit scores, and time periods.

> **Note:** This project uses synthetic data for educational and portfolio demonstration purposes. It does not represent real borrowers, financial institutions, or actual lending decisions.

## 🎯 Business Objectives

- Analyze loan distribution across risk categories.
- Measure loan defaults and the overall default rate.
- Evaluate default rate variations across employment categories.
- Compare loan amounts across different loan purposes.
- Track monthly changes in loan amounts.
- Explore observed default patterns across credit scores.
- Monitor total outstanding loan balances.
- Build an interactive dashboard for exploring loan portfolio metrics.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI | Dashboard development and data visualization |
| Power Query | Data cleaning and transformation |
| DAX | Measures and business calculations |
| CSV | Dataset storage and input |

## 📊 Dashboard Features

### Key Performance Indicators (KPIs)

- **Total Loans:** Number of distinct loans in the selected dataset.
- **Total Loan Amount:** Sum of the loan amounts.
- **Defaulted Loans:** Number of distinct loans classified as defaulted.
- **Default Rate:** Proportion of distinct loans classified as defaulted.
- **Total Outstanding Balance:** Sum of the outstanding loan balances.

### Visualizations

1. **Loan Distribution by Risk Category** — Examines the distribution of loans across Low, Medium, and High risk categories.
2. **Loans by Status** — Compares loans by repayment status.
3. **Total Loan Amount by Purpose** — Shows how loan value is distributed across loan purposes.
4. **Default Rate by Employment Status** — Compares observed default rates across employment categories.
5. **Monthly Loan Amount Trend** — Tracks changes in loan amounts across months.
6. **Default Rate by Credit Score** — Explores variations in observed default rates across credit scores.

### Interactive Filters

The dashboard includes slicers for:

- Loan Date
- Risk Category
- Employment Status
- Loan Purpose

These filters allow users to investigate selected segments of the portfolio and dynamically explore the report's metrics and visualizations.

## 📈 Key Business Insights

The dashboard supports the following areas of business analysis.

### 1. Loan Portfolio Risk Distribution

Analyze how loans are distributed across Low, Medium, and High risk categories. This helps identify the relative size of each risk segment and determine which segments may require closer monitoring.

### 2. Loan Default Performance

Compare the number of defaulted loans with the total loan portfolio and monitor the overall default rate. These measures provide a high-level view of observed repayment performance.

### 3. Default Rate by Employment Status

Compare default rates across Salaried, Self-Employed, Contract, and Unemployed borrowers. Differences between these groups can help identify patterns for further investigation, while accounting for the number of loans in each category.

### 4. Loan Amount by Purpose

Examine the total loan amount associated with purposes such as Debt Consolidation, Home Improvement, Auto, Education, Medical, and Small Business. This identifies which purposes account for relatively larger portions of the portfolio's loan value.

### 5. Monthly Loan Amount Trends

Analyze monthly changes in total loan amounts to identify periods of relatively higher or lower lending volume. These trends can support further investigation into changes in portfolio activity over time.

### 6. Default Rate by Credit Score

Explore how observed default rates vary across borrower credit scores. This can help identify potential patterns between credit scores and loan outcomes. Results should be interpreted carefully when individual score values have limited observations.

### 7. Outstanding Loan Exposure

Monitor total outstanding balances to understand the amount of loan value that remains unpaid. Considering outstanding balances alongside default metrics provides additional context for reviewing portfolio exposure.

### Business Value

The dashboard brings important portfolio metrics into a single interactive report. It enables users to:

- Compare loan risk segments and repayment outcomes.
- Identify employment categories with relatively higher observed default rates.
- Understand how loan amounts vary by purpose and month.
- Explore portfolio performance using interactive filters.
- Identify areas requiring deeper analysis and risk-monitoring investigation.

**Interpretation note:** These are the business questions and analytical areas supported by the dashboard, not claims of validated findings. Specific conclusions and numerical rankings should be documented after validating the complete dataset with report filters cleared. Observed relationships do not establish causation.

## 🧮 DAX Measures

The dashboard uses DAX measures to calculate key portfolio metrics.

### 1. Total Loans

Counts distinct loan IDs.

```DAX
Total Loans =
DISTINCTCOUNT(credit_risk_dataset[Loan_ID])
```

### 2. Total Loan Amount

Calculates the sum of loan amounts.

```DAX
Total Loan Amount =
SUM(credit_risk_dataset[Loan_Amount])
```

### 3. Defaulted Loans

Counts distinct loans with a status of `Defaulted`.

```DAX
Defaulted Loans =
CALCULATE(
    DISTINCTCOUNT(credit_risk_dataset[Loan_ID]),
    credit_risk_dataset[Loan_Status] = "Defaulted"
)
```

### 4. Default Rate

Calculates the proportion of distinct loans classified as defaulted.

```DAX
Default Rate =
DIVIDE(
    [Defaulted Loans],
    [Total Loans],
    0
)
```

Format this measure as a percentage in Power BI.

### 5. Total Outstanding Balance

Calculates the sum of outstanding loan balances.

```DAX
Total Outstanding Balance =
SUM(credit_risk_dataset[Outstanding_Balance])
```

## 📂 Project Structure

```text
Credit-Risk-Analysis/
│
├── Credit_Risk_Analysis.pbix
├── README.md
│
├── dataset/
│   └── credit_risk_dataset.csv
│
└── screenshots/
    └── dashboard.png
```

*The folder structure above represents the recommended repository organization. Upload the files using these names and locations, or update the structure to match your repository.*

## 🚀 How to Use

1. Clone or download this repository.
2. Open `Credit_Risk_Analysis.pbix` using Microsoft Power BI Desktop.
3. If Power BI requests the data source location, update the path to `dataset/credit_risk_dataset.csv`.
4. Refresh the data if required.
5. Use the slicers to explore different loan dates, risk categories, employment statuses, and loan purposes.
6. Review the KPIs and visualizations to investigate portfolio patterns.

## ⚠️ Data Disclaimer

This project uses synthetic practice data. Loan outcomes and risk categories are simulated and are not validated assessments of real credit risk.

The dashboard is intended for educational purposes, portfolio demonstration, and Power BI practice. Its results should not be used to approve or reject loans, evaluate real borrowers, or make financial decisions.

## 👨‍💻 Author

Created as a Data Analytics portfolio project to practice:

- Power BI dashboard development
- Data cleaning and transformation with Power Query
- DAX measures and calculations
- Interactive data visualization
- Business analysis and reporting

---

**If you find this project useful, consider giving the repository a ⭐ on GitHub.**
