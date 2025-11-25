# Customer Churn Prediction – End-to-End Data Analysis, BI & Machine Learning Project

## 📌 Project Overview

This project is an end-to-end Customer Churn Analysis & Prediction System built using SQL Server, Power BI, and Machine Learning (Python – Random Forest).
It covers the complete data lifecycle — ETL → Data Modeling → Dashboarding → ML Model → Prediction Visualization.

The project helps businesses:

- Understand key churn drivers
- Identify at-risk customers
- Improve customer retention
- Make data-driven decisions

1️⃣ ETL Pipeline (SQL Server)

- Imported raw CSV data into SQL Server using SSMS Import Wizard.
- Created staging (stg_Churn) and production (prod_Churn) tables.
- Cleaned null values using SQL transformations (ISNULL).
- Performed exploratory analysis:
   - Null checks
   - Distinct counts
   - Revenue distribution
   - State-wise customer distribution

- Created views for reporting:
   - vw_ChurnData - Churned/Stayed customers
   - vw_JoinData - Newly joined customers

2️⃣ Data Modeling & Power BI Transformations

Key transformations:
  - Added Churn Status flag (1 = Churned, 0 = Stayed)
  - Created:
     • Monthly Charge Range
     • Age Groups & sorting order
     • Tenure Groups & sorting order

  - Unpivoted service columns for service-wise churn patterns.

3️⃣ Power BI Dashboard

Created interactive dashboards with:

📌 Summary Metrics
   • Total Customers
   • New Joiners
   • Total Churn
   • Churn Rate

📌 Demographic Analysis
   • Gender vs Churn
   • Age Group distribution

📌 Geographical Insights
   • Churn by Top 5 States

📌 Account & Contract Insights
   • Tenure Groups
   • Contract Type
   • Payment Method

📌 Services & Churn
   • Internet Type
   • Add-on Services impact on churn

📌 Churn Reasons
   • Churn Category
   • Churn Reason (tooltip drill-down)

<img width="1905" height="777" alt="Sales Dashboard (2)" src="https://github.com/Sameer2615/Customer-Churn-Prediction/blob/main/Dashboard_images/Churn%20Analysis%20-%20Summary.png" />

4️⃣ Machine Learning – Churn Prediction (Python)

Built a predictive model using Random Forest Classifier.

✔ Model Steps:
- Data import from SQL views
- Categorical encoding using LabelEncoder
- Train-test split (80/20)
- Model training with RandomForestClassifier

Evaluation using:
- Confusion Matrix
- Classification Report
- Feature Importance Plot

✔ Predictive Output:
- Predicted churn for new joiners
- Output saved as a CSV

5️⃣ Power BI – Predicted Churn Dashboard
<img width="1905" height="777" alt="Sales Dashboard (2)" src="https://github.com/Sameer2615/Customer-Churn-Prediction/blob/main/Dashboard_images/Churn%20Analysis%20-%20Prediction.png" />
- Loaded the ML predictions back into Power BI to display:
- Predicted churners (Customer IDs)
- Revenue & refund patterns
- Tenure & contract type distribution
- Demographic insights
- State-wise predicted churn

🛠️ Tech Stack
Category	            Tools
Database & ETL  	SQL Server, SSMS
Business Intelligence	Power BI, DAX
Programming	      Python, Jupyter Notebook
ML Framework	Scikit-Learn
Libraries	Pandas, NumPy, Matplotlib, Seaborn, Joblib

📁 Files Included

- CHURN.pdf – Power BI Report / Documentation
- Churn_prediction.ipynb – ML Jupyter Notebook
- SQL Scripts (ETL + Views + Transformations)
- Power BI Dashboard (.pbix) (if uploaded)
- Prediction CSV 

🚀 Key Outcomes

- Built a complete churn analytics system from scratch.
- Delivered business-ready insights through a Power BI dashboard.
- Developed a high-performing Random Forest model to predict churn.
- Enabled organizations to take proactive retention actions.
