# AI Adoption & Business Impact Analytics

An end-to-end data analytics project analyzing AI adoption patterns, business performance, AI ROI, and AI maturity across companies from 2020–2025 using Python and Power BI.

## 📌 Project Overview

This project analyzes AI adoption and its business impact across a multi-dimensional dataset covering company information, industries, countries, financial performance, AI use cases, ROI, and AI maturity.

The project follows an end-to-end analytics workflow:

**Raw Data → Data Cleaning → Exploratory Data Analysis → Statistical Analysis → Power BI Dashboard → Business Insights**

The analysis was performed using Python for data exploration and visualization, followed by an interactive Power BI dashboard for business reporting and decision-making.

---

## 🎯 Objectives

- Analyze AI adoption trends across industries and countries.
- Identify major AI use cases adopted by companies.
- Analyze revenue trends from 2020 to 2025.
- Evaluate AI Return on Investment (ROI) across industries.
- Analyze AI maturity levels across companies.
- Compare companies based on industry, country, and company type.
- Build an interactive Power BI dashboard for business stakeholders.

---

## 🛠️ Technologies Used

### Programming & Data Analysis
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Business Intelligence
- Power BI Desktop
- DAX
- Power Query

### Data
- CSV
- Structured tabular data

---

## 📊 Dataset

The cleaned dataset contains:

| Metric | Value |
|---|---:|
| Total Records | 4,848 |
| Unique Companies | 1,000 |
| Years Covered | 2020–2025 |
| Average AI ROI | 25.06% |
| Average AI Maturity Score | 62.76 / 100 |
| Industries | 8 |
| Countries | 10 |
| Real Companies | 111 |
| Synthetic Company Records | 4,737 |

### Main Dataset Columns

- `Year`
- `Company`
- `Industry`
- `Country`
- `Company_Type`
- `Employee_Size`
- `Revenue_USD`
- `Uses_AI`
- `Use_Case`
- `AI_ROI_Percent`
- `AI_Maturity_Score`

> **Note:** The cleaned dataset is an AI-adopter-focused dataset, with all 4,848 cleaned records marked as `Uses_AI = Yes`.

---

## 🔍 Exploratory Data Analysis

EDA was performed using Python with Pandas, Matplotlib, and Seaborn.

The analysis covered:

### Industry Analysis
Analyzed company distribution across major industries including:

- Technology
- Finance
- Telecom
- E-commerce
- Manufacturing
- Retail
- Logistics
- Healthcare

### AI Use Case Analysis

Analyzed the frequency of AI use cases such as:

- Supply Chain Optimization
- Chatbots
- Customer Segmentation
- AI Trading
- Generative AI
- Other enterprise AI applications

### Revenue Analysis

Analyzed average company revenue trends between 2020 and 2025.

The highest average revenue recorded in the dataset was approximately **$18.3B in 2025**.

### AI ROI Analysis

Compared AI ROI across industries.

The average AI ROI was approximately **25.06%**, with relatively similar ROI values across industries.

### AI Maturity Analysis

Analyzed AI maturity scores ranging from **1 to 100**.

The overall average maturity score was approximately **62.76**.

### Geographic Analysis

Compared AI-adopting companies across countries, including:

- USA
- Canada
- Brazil
- China
- India

and other countries represented in the dataset.

---

## 📈 Power BI Dashboard

An interactive Power BI dashboard was developed to convert the analysis into business-friendly insights.

### Dashboard Features

- KPI cards
- Line charts
- Bar charts
- Donut charts
- Scatter plots
- Waterfall charts
- Gauge visual
- Slicers
- Drill-through
- Cross-filtering
- Interactive tooltips

### Dashboard Pages

#### 1. Overview

Provides high-level KPIs including:

- Total Companies
- AI Adoption %
- Revenue
- AI ROI
- AI Maturity

Designed for an executive-level overview.

#### 2. Detailed Analysis

Provides detailed analysis of:

- Industry performance
- AI use cases
- Revenue trends
- AI ROI
- Year-over-year trends

#### 3. Comparison

Provides comparative analysis based on:

- Company type
- Country
- Industry
- AI ROI
- AI maturity

#### 4. Dashboard Summary

Combines important visuals and KPIs into a quick business summary.

---

## 🧮 DAX Measures

The Power BI dashboard uses dynamic DAX measures rather than relying only on calculated columns.

### Total Companies

```DAX
Total Companies =
DISTINCTCOUNT('DUPLICATE'[Company])
