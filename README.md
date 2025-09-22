# HR Attrition Predictive Model for a Fintech Startup

### Project Overview

This project presents an end-to-end data science solution to a critical business problem: predicting and mitigating employee attrition. Using a synthetic dataset modeled on a high-growth fintech company, this project demonstrates a full-stack data analysis workflow, from initial data exploration to delivering actionable business recommendations.

### 1. Problem Statement

High employee turnover poses a significant risk to companies, leading to increased recruitment costs, loss of institutional knowledge, and disruption to team productivity. The objective of this project was to develop a machine learning model capable of identifying employees at high risk of leaving, allowing the People Team to intervene proactively and improve employee retention.

---

### 2. Methodology

The project was executed in a phased approach to ensure a robust and reliable solution:

* **Data Exploration & Analysis**: Performed comprehensive Exploratory Data Analysis (EDA) to uncover patterns and relationships between various HR metrics (e.g., salary, tenure, satisfaction) and attrition.
* **Data Preprocessing**: Cleaned the data by handling missing values and engineered a new feature, `SalaryPerTenure`, to better capture compensation trends over time. Categorical data was encoded, and features were scaled to prepare them for modeling.
* **Model Building**: Built and evaluated a **Logistic Regression** model as a baseline and a **Random Forest Classifier** for its superior predictive capabilities.
* **Model Refinement**: Addressed the critical issue of class imbalance using **SMOTE (Synthetic Minority Oversampling Technique)**, which significantly improved the model's ability to identify the "at-risk" employees.
* **Actionable Recommendations**: Extracted feature importance from the refined model to provide concrete, data-driven recommendations that the People Team can implement.

---

### 3. Key Findings & Results

The final, refined model provides a powerful tool for predicting attrition:

* **Improved Predictive Power**: The model's ability to correctly identify employees who left (**recall**) increased from **14%** to **29%** after using SMOTE. This makes the model far more valuable for proactive retention efforts.
* **Top Predictors of Attrition**: The model revealed the most influential factors driving attrition:
    1.  **CultureAlignmentScore**: The single most important predictor.
    2.  **TenureMonths**: The length of time an employee has been with the company.
    3.  **SalaryPerTenure**: The ratio of salary to tenure, indicating compensation growth.
    4.  **DistanceFromHome**: A strong indicator of work-life balance issues.

---

### 4. Actionable Recommendations

Based on these findings, I developed three core recommendations for the People Team:

* **Proactive Compensation Reviews**: Implement a program to review compensation for employees who have not received a promotion or salary increase in over 18 months.
* **Culture & Satisfaction Initiatives**: Utilize pulse surveys to regularly measure employee satisfaction and culture alignment, enabling early intervention for at-risk individuals.
* **Work-Life Balance Audits**: Encourage leaders to monitor overtime and champion the company's flexible work policies to prevent burnout, especially for long-tenured employees.

---

### 5. Technologies Used

* **Python**: The primary programming language.
* **Pandas**: For data manipulation and analysis.
* **Scikit-learn**: For machine learning modeling, preprocessing, and evaluation.
* **Matplotlib & Seaborn**: For data visualization.
* **Imblearn**: For handling class imbalance.
* **Git & GitHub**: For version control and project hosting.
