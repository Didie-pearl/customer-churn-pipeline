# End-to-End Customer Churn Intelligence Pipeline

## Project Overview
In the highly competitive telecommunications sector, retaining customers is as critical as acquiring new ones. This project implements a **production-grade data intelligence pipeline** designed to predict customer churn with high precision. By integrating automated ETL processes with advanced machine learning, the pipeline transforms raw customer data into prioritized retention strategies.

**Objective:** To reduce revenue loss by identifying high-risk customer segments and providing actionable data-driven recommendations for the customer success team.

---

## Technical Architecture & Workflow
The pipeline is built with a modular structure, ensuring each stage of the data lifecycle is handled with precision:

* **Data Ingestion & Audit:** Automated loading with structural integrity checks. Resolved a critical type mismatch for `TotalCharges` (Object to Float).
* **Robust Data Cleaning:** - **Missing Values:** Utilized **Median Imputation** for missing records because it is robust against outliers, ensuring the model remains unbiased by extreme values.
    - **Outlier Management:** Applied the **Interquartile Range (IQR) method** to validate data distribution; identified a highly consistent dataset with 0 statistical anomalies.
* **Feature Engineering:** - Conducted correlation analysis to identify key drivers; discovered a strong 0.83 correlation between tenure and total spend.
    - Implemented **Standardization (StandardScaler)** and Categorical Encoding.
* **Predictive Modeling:** - **Split Strategy:** 70% Training / 30% Testing.
    - **Experimental Approach:** Comparative analysis of Logistic Regression, Random Forest, and XGBoost.
* **Evaluation & Tuning:** Used **GridSearchCV** for hyperparameter optimization. The final **Logistic Regression** model achieved a champion accuracy of **81.07%**.

---

## 📊 Business Insights & Impact 
Based on the EDA and Feature Importance results, the following strategic insights were developed:

* **Incentivize Long-Term Loyalty:** "The business should incentivize long-term contracts through small discounts to lock in revenue."
    * *Evidence:* Month-to-month contracts were identified as the #1 churn driver.
* **The 'Danger Zone' Window:** "The first 12 months are the 'Danger Zone.' We need a high-touch onboarding program here."
    * *Evidence:* Data visualization confirmed a significant churn spike for customers with tenure < 1 year.
* **Price Sensitivity Analysis:** "Churn is price-sensitive. High-value customers feel the 'pinch' of high monthly bills more acutely."
    * *Evidence:* Model coefficients flagged Fiber Optic (the highest-priced tier) as a major risk factor.
* **Behavior Over Demographics:** "Demographics like gender are secondary; behavioral factors like contract type and billing are the primary levers for retention."
    * *Evidence:* Gender distribution was nearly identical for churned vs. stayed customers, proving demographics are not predictive in this segment.

    *   **Proposed Business Action:** Implement an automated "Loyalty Bridge" program that offers discounted 1-year contract upgrades to high-risk month-to-month customers within their first 6 months of tenure.

### 📈 Predictive Drivers
![Feature Importance]()

---

## Tech Stack & Skills
* **Languages:** Python (Pandas, NumPy)
* **Modeling:** Scikit-learn (Random Forest, Logistic Regression, XGBoost)
* **Visualization:** Matplotlib, Seaborn for stakeholder-ready insights
* **Environment:** Google Colab

---

## 🔗 Dataset
The analysis uses the [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) from Kaggle.

---

## Author
**Adedoyin Adesoji** *Data Analyst | Aspiring Data Scientist & ML Engineer* [![LinkedIn] https://www.linkedin.com/in/adedoyinadesoji
[![GitHub] 
https://github.com/Didie-pearl
