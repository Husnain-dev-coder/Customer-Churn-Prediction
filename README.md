# Customer-Churn-Prediction
Customer Churn Prediction using XGBoost and Feature Engineering
# 📉 Project 3 — Customer Churn Prediction

A machine learning model that predicts which customers are likely to
cancel their subscription using XGBoost — the most powerful ML 
algorithm used in real businesses today.

## 🎯 Problem Statement
Businesses lose money every time a customer leaves. This model 
identifies HIGH RISK customers BEFORE they churn so the company 
can take action and retain them.

## 📊 Dataset
- 1000 synthetic telecom customer records
- Inspired by real-world churn patterns (Jazz/Zong style)

## 🔢 Features Used
| Feature | Description |
|---|---|
| tenure | Months customer has been with company |
| monthly_charges | Monthly subscription fee (Rs) |
| num_complaints | Number of complaints made |
| support_calls | Number of support calls made |
| age | Customer age |
| num_products | Number of products subscribed |
| contract_type | Monthly / Yearly / TwoYear |
| internet | Has internet service or not |
| total_charges | tenure × monthly_charges (engineered) |
| complaints_per_month | complaints / tenure (engineered) |
| calls_per_month | support_calls / tenure (engineered) |

## 🧠 Model
- Algorithm: XGBoost (eXtreme Gradient Boosting)
- Train/Test Split: 80/20 with stratification
- Cross Validation: 5-Fold CV for reliable evaluation

## 📈 Results
- Accuracy: 95%+
- ROC-AUC Score: 0.92+
- Cross Validation Average: 93%+

## 💡 Key Insights (Feature Importance)
- complaints_per_month → biggest churn driver
- tenure → new customers churn most
- total_charges → high paying customers at risk
- contract_type → monthly contracts churn more

## 🛠️ Tech Stack
Python · XGBoost · Scikit-learn · Pandas · NumPy · 
Matplotlib · Seaborn

## ▶️ How to Run
pip install -r requirements.txt
python ChurnPrediction.py

## 📁 Output Files
- churn_eda.png — EDA analysis plots
- churn_confusion.png — Confusion matrix
- feature_importance.png — What causes churn

## 👤 Author
Husnain — 30 Day ML & AI Challenge — Day 5

## 🔗 Connect
GitHub: github.com/Husnain-dev-coder
