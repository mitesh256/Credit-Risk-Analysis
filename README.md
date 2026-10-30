# Credit Risk Analysis Dashboard | Power BI

**Power BI • Power Query • DAX • Data Analytics • Credit Risk Analysis**

An interactive Power BI dashboard designed to analyze loan portfolio performance, understand credit risk distribution, identify default patterns, and monitor outstanding loan exposure.

This project explores loan performance across different employment statuses, loan purposes, credit score bands, debt-to-income ratios, and risk categories using interactive visualizations and DAX-based KPIs.

> **Dataset Disclaimer:** This project uses synthetic practice data for educational and portfolio demonstration purposes. It does not represent real borrowers, financial institutions, or actual lending decisions.

---

## 📑 Table of Contents

1. [About This Project](#1-about-this-project)
2. [Problem Statement](#2-problem-statement)
3. [Business Questions](#3-business-questions)
4. [Project Objectives](#4-project-objectives)
5. [Dataset Overview](#5-dataset-overview)
6. [Project Structure](#6-project-structure)
7. [Project Methodology](#7-project-methodology)
8. [Dashboard Features](#8-dashboard-features)
9. [Dashboard Screenshots](#9-dashboard-screenshots)
10. [DAX Measures](#10-dax-measures)
11. [Key Business Findings](#11-key-business-findings)
12. [Business Recommendations](#12-business-recommendations)
13. [Technical Specifications](#13-technical-specifications)
14. [How to Use the Project](#14-how-to-use-the-project)
15. [Challenges and Solutions](#15-challenges-and-solutions)
16. [Limitations](#16-limitations)
17. [Skills Demonstrated](#17-skills-demonstrated)
18. [Author](#18-author)

---

## 1. About This Project

Credit risk analysis is an important part of financial and lending operations. Financial institutions need to evaluate loan portfolios, monitor repayment behaviour, and understand potential default risks.

This project uses Microsoft Power BI to analyze loan portfolio data and identify patterns related to loan defaults, credit scores, employment status, loan purposes, and outstanding balances.

The dashboard combines data transformation using Power Query, KPI calculations using DAX, and interactive visualizations to present important credit risk indicators.

**The main focus of this project is to:**

- Understand overall loan portfolio performance.
- Analyze loan distribution across different risk categories.
- Identify patterns in loan defaults.
- Compare default rates across employment categories.
- Explore credit score and debt-to-income patterns.
- Monitor loan amounts and outstanding balances.
- Generate meaningful business insights and recommendations.

---

## 2. Problem Statement

Lending institutions face the challenge of managing loan portfolios while monitoring repayment performance and potential credit risk.

Analyzing only total loan amounts or default counts does not provide a complete understanding of portfolio performance.

Businesses need to understand:

- How are loans distributed across different risk categories?
- What proportion of loans are classified as defaulted?
- Which employment categories have higher observed default rates?
- Which loan purposes account for larger loan amounts?
- How do credit scores relate to observed default patterns?
- How does debt-to-income ratio relate to loan defaults?
- How much loan balance remains outstanding?

This project uses Power BI to explore these questions and provide a consolidated view of loan portfolio performance.

---

## 3. Business Questions

The dashboard focuses on answering the following business questions:

| No. | Business Question |
|---|---|
| 01 | What is the total loan amount and total number of loans? |
| 02 | What is the overall loan default rate? |
| 03 | How are loans distributed across Low, Medium, and High risk categories? |
| 04 | Which employment categories have higher observed default rates? |
| 05 | Which loan purposes account for the largest loan amounts? |
| 06 | How does the default rate vary across credit score bands? |
| 07 | How does default behaviour vary across debt-to-income ratio groups? |
| 08 | What is the total outstanding loan balance? |
| 09 | How do loan amounts change over time? |

---

## 4. Project Objectives

- Analyze overall loan portfolio performance.
- Calculate important credit risk KPIs.
- Understand loan distribution across risk categories.
- Compare default rates across employment categories.
- Evaluate loan amounts by purpose.
- Explore default patterns across credit score bands.
- Analyze debt-to-income ratio and default behaviour.
- Monitor outstanding loan exposure.
- Develop an interactive Power BI dashboard.
- Generate business insights and recommendations.

---

## 5. Dataset Overview

The project uses a synthetic credit risk dataset containing loan-related information, borrower characteristics, financial indicators, and repayment status.

### Dataset Information

| Attribute | Details |
|---|---|
| Dataset Name | Credit Risk Dataset |
| File Format | CSV |
| Data Source | Synthetic Practice Dataset |
| Analysis Tool | Microsoft Power BI |
| Data Transformation | Power Query |
| Business Calculations | DAX |
| Analysis Type | Descriptive Analytics |

### Key Dataset Attributes

| Column | Description |
|---|---|
| Loan_ID | Unique loan identifier |
| Loan_Amount | Amount of the loan |
| Loan_Status | Repayment status |
| Risk_Category | Assigned loan risk category |
| Employment_Status | Borrower's employment category |
| Loan_Purpose | Purpose of the loan |
| Credit_Score | Borrower's credit score |
| Debt_to_Income_Ratio | Debt-to-income ratio |
| Outstanding_Balance | Remaining loan balance |
| Loan_Date | Loan date |

The dataset supports analysis of portfolio distribution, repayment status, borrower segments, and loan exposure.

---

## 6. Project Structure

```text
Credit-Risk-Analysis/
│
├── CREDIT ANALYSIS.pbix
│
├── credit_risk_dataset.csv
│
├── Screenshot 2026-10-30 122102.png
│
├── Business_Insights.png
│
└── README.md
```

---

## 7. Project Methodology

### 1. Data Loading

The credit risk dataset was imported into Microsoft Power BI using a CSV data source.

The dataset contains loan information, borrower characteristics, financial indicators, and repayment status.

### 2. Data Cleaning and Transformation

Power Query was used as part of the data preparation process.

The preparation workflow includes:

- Reviewing dataset columns and data types.
- Preparing fields for analysis.
- Checking important loan and borrower attributes.
- Organizing data for dashboard reporting.

### 3. DAX Measure Development

DAX measures were developed to calculate important business KPIs.

These measures support dynamic calculations and respond to dashboard filters.

### 4. Dashboard Development

Power BI visualizations were created to analyze:

- Loan portfolio KPIs.
- Risk category distribution.
- Monthly loan amount trends.
- Default rates across borrower segments.
- Loan amount distribution by purpose.
- Loan repayment status.

### 5. Business Analysis

The dashboard findings were interpreted to identify borrower segments and loan portfolio areas that may require further investigation.

---

## 8. Dashboard Features

### A. Key Performance Indicators (KPIs)

The dashboard includes five major KPI cards:

| KPI | Description |
|---|---|
| Total Loan Amount | Sum of loan amounts |
| Total Loans | Distinct count of loan IDs |
| Default Rate | Percentage of loans classified as defaulted |
| Total Outstanding Balance | Sum of outstanding loan balances |
| Defaulted Loans | Number of distinct defaulted loans |

### B. Loan Distribution by Risk Category

A donut chart compares loan distribution across:

- Low Risk
- Medium Risk
- High Risk

This visualization helps understand the composition of the loan portfolio.

### C. Monthly Loan Amount Trend

A line chart tracks monthly loan amounts to identify changes in lending activity over time.

### D. Default Rate by Employment Status

A column chart compares observed default rates across:

- Unemployed
- Contract
- Salaried
- Self-Employed

### E. Default Rate by Loan Purpose

A horizontal bar chart compares default rates across different loan purposes.

### F. Total Loan Amount by Purpose

This visualization compares loan amounts across:

- Debt Consolidation
- Home Improvement
- Auto
- Education
- Medical
- Small Business

### G. Default Rate by Credit Score Band

The chart explores how default rates vary across credit score categories:

- 580–669
- Below 580
- 670–739
- 740+

### H. Default Rate by Debt-to-Income Ratio

This visualization examines default patterns across debt-to-income ratio groups.

### I. Loans by Status

A bar chart compares loans by repayment status, including:

- Repaid/Current
- Defaulted
- Late

### J. Interactive Filters

The dashboard includes slicers for:

- Employment Status
- Loan Purpose
- Risk Category
- Loan Date

These filters allow users to explore different portfolio segments dynamically.

---

## 9. Dashboard Screenshots

### Credit Risk Analysis Dashboard

The main dashboard provides an overview of loan portfolio performance, default rates, risk distribution, loan purposes, employment categories, and outstanding balances.

![Credit Risk Analysis Dashboard](Screenshot%202026-10-30%20122102.png)

### Business Insights and Recommendations

The business insights report summarizes important findings and potential actions related to credit scores, employment status, loan purposes, and portfolio exposure.

![Business Insights and Recommendations](Business_Insights.png)

---

## 10. DAX Measures

The dashboard uses DAX measures to calculate key portfolio metrics.

### 1. Total Loans

Counts the distinct number of loan IDs.

```dax
Total Loans =
DISTINCTCOUNT(
    credit_risk_dataset[Loan_ID]
)
```

### 2. Total Loan Amount

Calculates the total loan amount.

```dax
Total Loan Amount =
SUM(
    credit_risk_dataset[Loan_Amount]
)
```

### 3. Defaulted Loans

Counts distinct loans classified as Defaulted.

```dax
Defaulted Loans =
CALCULATE(
    DISTINCTCOUNT(
        credit_risk_dataset[Loan_ID]
    ),
    credit_risk_dataset[Loan_Status] = "Defaulted"
)
```

### 4. Default Rate

Calculates the percentage of distinct loans classified as defaulted.

```dax
Default Rate =
DIVIDE(
    [Defaulted Loans],
    [Total Loans],
    0
)
```

Format this measure as a percentage in Power BI.

### 5. Total Outstanding Balance

Calculates the total outstanding loan balance.

```dax
Total Outstanding Balance =
SUM(
    credit_risk_dataset[Outstanding_Balance]
)
```

---

## 11. Key Business Findings

The following observations are based on the displayed dashboard and business insights report.

### 1. Credit Score and Default Risk

- The 580–669 credit score band shows the highest observed default rate, at approximately 39%.
- The 740+ credit score band shows a lower observed default rate of approximately 15%.

**Business Interpretation:**

Lower credit score groups show higher observed default rates in the displayed analysis. Credit score segmentation can help identify areas requiring further investigation.

### 2. Employment Status and Default Risk

- Unemployed borrowers show an observed default rate of approximately 44%.
- Self-employed borrowers show an observed default rate of approximately 26%.

**Business Interpretation:**

Employment categories show differences in observed default rates and may require further portfolio investigation.

### 3. Loan Purpose and Default Risk

- Small Business loans show an observed default rate of approximately 33%.
- Debt Consolidation loans show an observed default rate of approximately 27%.

**Business Interpretation:**

Default rates vary across loan purposes, highlighting the importance of evaluating repayment capacity across different loan segments.

### 4. Loan Portfolio Distribution

Debt Consolidation accounts for the largest total loan amount among the displayed loan purposes.

**Business Interpretation:**

A substantial portion of the displayed portfolio exposure is associated with Debt Consolidation loans.

### 5. Overall Portfolio KPIs

The dashboard screenshot displays the following KPI values:

| Metric | Displayed Value |
|---|---:|
| Total Loan Amount | $24.2983M |
| Total Loans | 2K |
| Default Rate | 29.07% |
| Total Outstanding Balance | $5.82M |
| Defaulted Loans | 491 |

The Total Loans card uses rounded display units. Exact figures should be obtained from the underlying Power BI measure.

> **Note:** These are dashboard snapshot values. They may change when users apply different slicer selections. The business insights percentages are approximate displayed values, not independently validated results for every possible filter context.

---

## 12. Business Recommendations

Based on the observed dashboard patterns, the following recommendations can be considered.

### 1. Strengthen Credit Assessment

Review credit assessment procedures for borrowers in the 580–669 credit score band. Consider additional affordability checks and risk-based review criteria rather than relying on credit scores alone.

### 2. Improve Monitoring for Unemployed Borrowers

Investigate repayment capacity and income stability among unemployed borrowers. Consider appropriate repayment support and early-warning monitoring within applicable lending policies.

### 3. Review Small Business Loan Risk

Evaluate repayment patterns and affordability assessments for Small Business loans. Review loan terms and borrower cash-flow information before making risk-management decisions.

### 4. Monitor Debt Consolidation Portfolio Exposure

Because Debt Consolidation represents the largest total loan amount among the displayed purposes, monitor its outstanding exposure, delinquency patterns, and default rates together.

### 5. Track Risk Indicators Regularly

Monitor default rates by credit score, employment status, debt-to-income ratio, and loan purpose. Review changes over time to identify segments requiring further investigation.

These recommendations are analytical suggestions based on the displayed synthetic data. They do not establish causal relationships or guarantee improvements in loan performance.

---

## 13. Technical Specifications

| Component | Technology / Approach |
|---|---|
| Dashboard Development | Microsoft Power BI |
| Data Source | CSV |
| Data Transformation | Power Query |
| Business Calculations | DAX |
| Aggregation | SUM() |
| Distinct Counting | DISTINCTCOUNT() |
| Conditional Calculation | CALCULATE() |
| Division and Error Handling | DIVIDE() |
| Data Visualization | Power BI Charts |
| Reporting | Interactive Dashboard |

---

## 14. How to Use the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/mitesh256/Credit-Risk-Analysis.git
```

### Step 2: Open the Project Folder

```bash
cd Credit-Risk-Analysis
```

### Step 3: Open Power BI Dashboard

Open `CREDIT ANALYSIS.pbix` using Microsoft Power BI Desktop.

### Step 4: Configure the Data Source

If Power BI requests the dataset location, update the source path to:

```text
credit_risk_dataset.csv
```

### Step 5: Refresh the Data

Refresh the dataset if required to load the data.

### Step 6: Explore the Dashboard

Use the interactive slicers to investigate:

- Employment Status
- Loan Purpose
- Risk Category
- Loan Date

Review the KPI cards, charts, and business insights to understand portfolio patterns.

---

## 15. Challenges and Solutions

The project involves several analytical areas that require careful consideration.

| Challenge | Approach |
|---|---|
| Understanding loan portfolio performance | Developed KPI cards for loan amount, total loans, default rate, and outstanding balance |
| Comparing different borrower segments | Used category-wise default rate visualizations |
| Understanding risk distribution | Created a donut chart for Low, Medium, and High risk categories |
| Exploring monthly loan trends | Developed a monthly loan amount line chart |
| Calculating business metrics | Used DAX measures for aggregations and conditional calculations |
| Making the report interactive | Added slicers for employment status, loan purpose, risk category, and loan date |

---

## 16. Limitations

- The dataset is synthetic and intended for educational purposes.
- The analysis is limited to the available dataset attributes.
- Observed relationships do not establish causation.
- Default rates can change depending on applied dashboard filters.
- The project does not validate actual borrower creditworthiness.
- Dashboard findings should not be used for real lending or loan approval decisions.
- The project focuses on descriptive analytics rather than predictive credit risk modelling.

---

## 17. Skills Demonstrated

- Microsoft Power BI
- Power Query
- DAX Measures
- Data Cleaning and Transformation
- KPI Development
- Credit Risk Analysis
- Loan Portfolio Analysis
- Default Rate Analysis
- Data Visualization
- Interactive Dashboard Development
- Business Insights
- Business Recommendations
- Analytical Problem Solving

---

## 18. Author

**Mitesh Suthar**

Aspiring Data Analyst | Power BI | SQL | Python | Excel

- GitHub: [mitesh256](https://github.com/mitesh256)

**Project Type:** Data Analytics Portfolio Project

**Tools:** Microsoft Power BI, Power Query, DAX

**Dataset:** Synthetic Credit Risk Dataset

---

*Turning loan portfolio data into meaningful credit risk insights.*

⭐ If you find this project useful, feel free to explore the repository.
