# Customer Churn Intelligence Pipeline
# End-to-End Customer Churn Intelligence Pipeline

## Project Overview
In the highly competitive telecommunications sector, retaining customers is as critical as acquiring new ones. This project implements a **production-grade data intelligence pipeline** designed to predict customer churn with high precision. By integrating automated ETL processes with advanced machine learning, the pipeline transforms raw customer data into prioritized retention strategies.

**Objective:** To reduce revenue loss by identifying high-risk customer segments and providing actionable data-driven recommendations for the customer success team.

---

##  Technical Architecture
The pipeline is designed with modularity and scalability in mind, adhering to modern software engineering principles:

* **Data Ingestion:** Automated handling of the Telco dataset, including schema validation.
* **Preprocessing Engine:** Robust cleaning protocols for handling inconsistent types (e.g., `TotalCharges` as object) and missing value imputation.
* **Feature Intelligence:** Engineering of behavioral metrics and categorical encoding (Label & One-Hot) to maximize model signal.
* **Predictive Modeling:** Implementation of a tuned **Random Forest Classifier** with cross-validation to ensure generalization.
* **Insights Layer:** Generation of feature importance scores to bridge the gap between model "black boxes" and business logic.

---

## Tech Stack & Skills
* **Languages:** Python (Pandas, NumPy)
* **Modeling:** Scikit-learn (Random Forest, Preprocessing, Metrics)
* **Database Logic:** SQL for initial data exploration and cohort analysis
* **Visualization:** Matplotlib, Seaborn for stakeholder-ready insights
* **Environment:** VS Code, Git for version control

---

## 📊 Business Insights & Impact
The model successfully identified that the most significant drivers of churn are:
1.  **Contract Type:** Customers on Month-to-Month contracts have a significantly higher churn rate compared to those on One-year or Two-year plans.
2.  **Tenure:** New customers are at the highest risk, suggesting a need for enhanced onboarding programs.
3.  **Charge Density:** High monthly charges relative to tenure act as a primary churn trigger.

**Proposed Business Action:** Implement an automated "Loyalty Bridge" program that offers discounted 1-year contract upgrades to high-risk month-to-month customers within their first 6 months of tenure.

---

## 🧩 Engineering Challenges & Learning
* **Data Type Integrity:** Handled numerical columns formatted as strings to prevent pipeline crashes during training.
* **Modularization:** Reconstructed a linear notebook into a functional Python pipeline to improve maintainability.
* **Class Imbalance:** Evaluated model performance using F1-score and Recall, recognizing that missing a potential churner (False Negative) is more costly than a false alarm.

---

## Dataset
The analysis uses the [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) from Kaggle. It contains information about a fictional telco company that provided home phone and Internet services to 7,043 customers in California.

---

## 👤 Author
**Adedoyin Adesoji** *Data Analyst | Aspiring Data Scientist & ML Engineer* [![LinkedIn] https://www.linkedin.com/in/adedoyinadesoji
[![GitHub] 
https://github.com/Didie-pearl
