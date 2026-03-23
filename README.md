# End-to-End Customer Churn Intelligence Pipeline

## Project Overview
In the highly competitive telecommunications sector, retaining customers is as critical as acquiring new ones. This project implements a **production-grade data intelligence pipeline** designed to predict customer churn with high precision. By integrating automated ETL processes with advanced machine learning, the pipeline transforms raw customer data into prioritized retention strategies.

**Objective:** To reduce revenue loss by identifying high-risk customer segments and providing actionable data-driven recommendationsfor the customer success team.

---

## Technical Architecture & Workflow
The pipeline is built with a modular structure, ensuring each stage of the data lifecycle is handled with precision. The pipeline is designed with modularity and scalability in mind, adhering to modern software engineering principles:

* **Data Ingestion & Audit:** Automated loading with structural integrity checks (schema validation and unique value analysis).
* **Robust Data Cleaning:** - Handling structural errors and inconsistent data types (e.g., `TotalCharges`).
    - **Outlier Management:** Using the **Interquartile Range (IQR) method** to identify and neutralize statistical anomalies.
* **Feature Engineering:** - Correlation analysis to identify key churn drivers.
* **Feature Intelligence:** Engineering of behavioral metrics and categorical encoding (Label & One-Hot) to maximize model signal.
    - Implementation of **Feature Scaling** (Standardization/Normalization) and categorical encoding.
* **Predictive Modeling:** - **Split Strategy:** 70% Training / 30% Testing to ensure robust model evaluation.
    - **Experimental Approach:** Comparative analysis of multiple algorithms to optimize for precision and recall.
* **Evaluation & Tuning:** Using Confusion Matrices and F1-mapping to bridge the gap between model "black boxes" and business logic.

---

## Tech Stack & Skills
* **Languages:** Python (Pandas, NumPy)
* **Modeling:** Scikit-learn (Random Forest, Logistic Regression, XGBoost)
* **Visualization:** Matplotlib, Seaborn for stakeholder-ready insights
* **Environment:** Google Colab

---

## 📊 Business Insights & Impact
The model successfully identified that the most significant drivers of churn are:
1.  **Contract Type:** Customers on Month-to-Month contracts have a significantly higher churn rate compared to those on One-year or Two-year plans.
2.  **Tenure:** New customers are at the highest risk, suggesting a need for enhanced onboarding programs.
3.  **Charge Density:** High monthly charges relative to tenure act as a primary churn trigger.

**Proposed Business Action:** Implement an automated "Loyalty Bridge" program that offers discounted 1-year contract upgrades to high-risk month-to-month customers within their first 6 months of tenure.

---

## Dataset
The analysis uses the [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) from Kaggle. It contains information about a fictional telco company that provided home phone and Internet services to 7,043 customers in California.

---

## Author
**Adedoyin Adesoji** *Data Analyst | Aspiring Data Scientist & ML Engineer* [![LinkedIn] https://www.linkedin.com/in/adedoyinadesoji
[![GitHub] 
https://github.com/Didie-pearl
