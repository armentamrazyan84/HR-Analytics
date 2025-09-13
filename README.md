# HR-Analytics
Uncovering insights to find reasons for employee attrition.

HR Attrition Analysis

Project Overview

This project analyzes employee attrition patterns using the IBM HR Employee Attrition dataset. The goal is to identify key factors influencing attrition and generate insights that can be visualized in Power BI

and explored statistically in R.

Tools & Languages

R (for statistical analysis, hypothesis testing, and visualization)

Power BI (for dashboards, KPIs, and interactive exploration)

Excel/CSV (dataset storage and cleaning)

Dataset

Source: IBM HR Analytics Employee Attrition Dataset

Rows: ~1,470 employees

Key variables:

Attrition (Yes/No) – Target variable

Demographics: Age, Gender, MaritalStatus, EducationField

Work-related: Department, JobLevel, OverTime, YearsAtCompany

Compensation: MonthlyIncome, PercentSalaryHike

Performance: PerformanceRating


Analyses Performed

Descriptive Statistics

- Overall attrition rate

- Attrition by department, job level, overtime, gender, marital status, tenure


Hypothesis Testing

- Chi-square tests for association between attrition and categorical variables (Department, OverTime, JobLevel, etc.)

- Independent-samples t-test for salary differences by overtime status


Correlation Analysis

- Explored relationships between numeric variables (e.g., JobLevel ↔ MonthlyIncome, Age ↔ TotalWorkingYears)


Interaction Effects

- Logistic regression to test whether the effect of overtime on attrition depends on:

   Gender → No significant moderation

   Job Level → Significant moderation (overtime affects junior staff more)

   YearsAtCompany (Tenure) → Overtime is most risky in early career



Visualizations (R)

Heatmaps: Attrition risk by OverTime × JobLevel, and OverTime × Tenure Group

Bar and line charts for attrition trends



Power BI KPIs

Overall Attrition Rate

Overtime Attrition Rate

Attrition Rate by Job Level

Average Monthly Income (with overtime vs non-overtime comparison)

Tenure-Based Attrition (≤ 3 years)



Key Insights

Overtime is the strongest predictor of attrition: employees working overtime are far more likely to leave.

Job level matters: junior employees are especially vulnerable when required to work overtime.

Early tenure (≤3 years) is a high-risk period, especially when combined with overtime.

Marital status: single employees are more likely to leave.

Department and gender have little effect on attrition.

Compensation is tied to job level and experience, but not to overtime. Employees who work overtime earn the same as those who don’t, which may explain why overtime drives attrition.



How to Use
R Scripts: Run the provided R code to reproduce statistical tests and heatmaps.
Power BI Dashboard: Load the DAX measures and visuals to explore KPIs interactively.
Report: Combine the insights and visuals for HR strategy discussions.
