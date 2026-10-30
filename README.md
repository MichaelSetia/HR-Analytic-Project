# 📊 HR Analytics & Compensation Review Project

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-green.svg)](https://seaborn.pydata.org/)

An end-to-end HR Data Analysis project focused on evaluating employee compensation fairness, salary band compliance, performance score distributions, and financial gap analysis across departments and locations.

---

## 🚀 Project Overview
In this project, employee records are analyzed to uncover insights regarding salary distribution relative to established department salary bands (Minimum and Maximum limits). The analysis helps HR management identify financial discrepancies, specifically quantifying total **overpaid** and **underpaid** compensation amounts, and tests whether employee performance scores correlate significantly with compensation levels.

---
## 📊 Dashboard Preview

<img width="523" height="391" alt="Screenshot 2026-10-29 at 11 49 57" src="https://github.com/user-attachments/assets/8f20d0ab-0cb2-4d94-a9b5-09b2c49189fd" />


## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation & Cleaning:** Pandas, NumPy
* **Statistical Analysis:** SciPy (`scipy.stats`)
* **Data Visualization:** Matplotlib, Seaborn
* **Dashboard:** Google Data Studio

---

## 📁 Dataset Structure
The dataset (`Employee_dataset.xlsx`) consists of two primary sheets:
1. **Sheet1 (Employee Data):** Contains employee demographics, job status, department, location, join dates, performance scores, remote work status, and current salary.
2. **SALARY (Salary Bands):** Defines the minimum and maximum standard salary thresholds for each department.

---

## 📈 Key Analysis & Insights

### 1. Salary Band & Gap Analysis
* **Underpaid Gap (Correction Cost):** Calculated total deficits for employees earning below their department's minimum salary band (Total Underpaid: **~$2.46M**). Departments like DevOps and Cloud Tech exhibit significant under-band gaps.
* **Overpaid Gap:** Calculated total excesses for employees earning above their department's maximum salary band (Total Overpaid: **~$5.00M**), notably concentrated in Admin and HR departments.

### 2. Performance vs. Compensation
* Conducted **One-Way ANOVA** testing to evaluate whether average salaries differ significantly across performance tiers (*Average, Good, Excellent, Poor*).
* **Finding ($p = 0.671$):** There is no statistically significant difference in average salary across different performance score tiers, indicating potential alignment gaps in merit-based pay structures.

### 3. Geographic & Departmental Distribution
* Analyzed average salaries across various department locations (California, Florida, Illinois, Nevada, New York, Texas).
* ANOVA testing across locations ($p = 0.632$) shows salary distribution remains relatively uniform across geographic regions.

---

## 🔍 Exploratory Data Analysis (EDA) Highlights
* **Data Cleaning:** Handled missing/unnecessary columns, standardized date formats, and mapped department salary benchmarks using left-joins.
* **Visualizations:** Utilized boxplots for outlier detection (Age & Salary), count plots for categorical distributions, heatmaps for cross-tabulated salary standards vs. performance scores, and customized currency-formatted bar charts.

---

## 📂 Repository Structure
```text
├── Employee_dataset.xlsx    # Raw dataset (Employee records & Salary bands)
├── EDA.ipynb                # Main Jupyter Notebook containing complete EDA & statistical analysis
└── README.md                # Project documentation
