# Telecom Customer Churn Analysis & Prediction

An end-to-end data analytics and machine learning project focused on understanding customer churn, identifying high-risk customer segments, and developing actionable business recommendations.

The project combines Python-based exploratory data analysis, machine learning, statistical hypothesis testing, and an interactive Power BI dashboard.

## 🚀 Live Demo

**Streamlit Application:** [Launch the Churn Prediction App](https://telecom-churn-project-files-8pna38bxqrqbxetvbwq3tg.streamlit.app/)

The application allows users to enter customer information and receive a churn prediction using the trained machine learning pipeline.

---

## 1. Business Problem

Customer churn is a major challenge for telecommunications companies. Losing existing customers can affect revenue, customer lifetime value, and long-term business growth.

The objective of this project is to:

- Understand customer churn patterns.
- Identify customer segments associated with higher churn.
- Develop a machine learning model to predict customer churn.
- Statistically investigate the relationship between early-tenure monthly charges and churn.
- Present actionable insights through an interactive Power BI report.

## 2. Dataset

**Dataset:** IBM Telco Customer Churn

- Total records: 7,043 customers
- Total features: 21 columns
- Target variable: Churn (Yes/No)

The dataset contains customer demographics, account information, subscribed services, contract details, payment methods, and billing information.

## 3. Exploratory Data Analysis

Performed exploratory data analysis using Python to understand customer behaviour and identify potential churn patterns.

Key areas investigated:

- Customer tenure and churn distribution.
- Monthly and total charges.
- Contract types and payment methods.
- Internet service and additional service adoption.
- Differences between churned and retained customers.

## 4. Machine Learning & Model Evaluation

Developed and evaluated multiple classification models to predict customer churn.

The final deployed pipeline uses:

**Logistic Regression with SMOTENC**

The pipeline includes preprocessing, categorical encoding, handling of class imbalance, and classification.

The trained pipeline was saved using Joblib and integrated into a Streamlit application.

## 5. Statistical Hypothesis Testing

Conducted a two-proportion Z-test to investigate whether early-tenure customers with higher monthly charges have a higher churn rate.

**Research question:**

Are customers with higher monthly charges during their first 12 months more likely to churn?

**Customer segmentation:**

- High-charge group: Monthly charges above $55.90.
- Low-charge group: Monthly charges at or below $55.90.
- Customer tenure: 12 months or less.

**Key findings:**

| Metric | Result |
|---|---:|
| High-charge churn rate | 62.73% |
| Low-charge churn rate | 32.18% |
| Difference | 30.55 percentage points |
| Z-statistic | 14.3039 |
| P-value | 1.03 × 10⁻⁴⁶ |
| 95% confidence interval | 26.50–34.46 percentage points |

**Conclusion:** Reject the null hypothesis at a 5% significance level. The analysis provides statistically significant evidence that early-tenure customers in the high-charge group have a higher churn rate.

This finding indicates an association, not proof of causation.

## 6. Power BI Dashboard — Veyra Telecom

Developed a three-page interactive Power BI report to communicate customer churn patterns, identify potential churn drivers, and present statistical findings.

### Page 1 — Churn Overview

Overall customer churn performance, customer distribution, contract types, internet services, monthly charges, and tenure.

### Page 2 — Churn Drivers

Analysis of churn by service adoption and payment method, supported by KPI cards and business takeaways.

### Page 3 — Early-Tenure Risk & Hypothesis Testing

Comparison of high-charge and low-charge customer churn rates, statistical test results, confidence interval, conclusion, and business recommendations.

**Dashboard Screenshots**



## 7. Streamlit Application

The machine learning model is deployed using Streamlit Community Cloud.

Application features:

- Customer information input form.
- Churn prediction.
- Interactive user interface.
- Trained Logistic Regression pipeline with SMOTENC.

## 8. Technologies Used

| Category | Tools |
|---|---|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, Imbalanced-learn |
| Statistical Analysis | SciPy |
| Business Intelligence | Power BI, DAX, Power Query |
| Deployment | Streamlit Community Cloud |
| Version Control | Git, GitHub |

## 9. Business Recommendations

Based on the analysis:

- Investigate early-tenure customers with higher monthly charges.
- Review the value proposition of high-priced plans.
- Examine the relationship between service adoption and churn.
- Investigate the payment experience of electronic-check customers.
- Explore targeted onboarding and customer retention initiatives.

These are proposed business actions based on observed associations and should be validated through further testing.

## 10. Project Structure

- Python notebooks for EDA, preprocessing, model evaluation, and hypothesis testing.
- Streamlit application files.
- Trained machine learning pipeline.
- Power BI report and dashboard screenshots.
- Project documentation.

---

**Project Status:** Completed

**Project Type:** End-to-End Data Analytics & Machine Learning Portfolio Project
