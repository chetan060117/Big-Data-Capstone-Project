# Project Title:

Credit Risk Prediction using PySpark ML on Databricks

# 1. Introduction

This project aims to build a machine learning model to predict the likelihood of a customer defaulting on their credit card payment next month. The dataset used is the UCI Credit Card Dataset containing 30,000 customer records.

# 2. Objective

Predict customer defaults using machine learning.

Segment customers based on financial behavior.

Model explainability

Create automated alerts for risky customers.

Recommend optimal credit limits.

# 3. Tools and Technologies

Platform: Databricks Free Edition

Language: Python (PySpark)

Libraries: PySpark MLlib, Pandas, Matplotlib


# 4. Architecture

Medallion Architecture (3 Layers):

Bronze Layer: Data ingestion (raw CSV → Delta table).

Silver Layer: Data cleaning, encoding, and feature engineering.

Gold Layer: Model predictions, alerts, and recommendations.

# 5. Methodology

Data Loading and Schema Definition

Data Cleaning & Feature Transformation

Model Building (Logistic Regression, Random Forest, etc.)

Evaluation (Accuracy, AUC, Confusion Matrix)

Model explainability

Clustering for Customer Segmentation

Alert System Implementation

Credit Limit Simulation & Optimization

# 6. Insights

Early warning system:

Customers showing payment delay in consecutive months (PAY_1–PAY_3) are 2–3x more likely to default.

Credit limit strategy:

Customers with lower LIMIT_BAL but high BILL_AMT show higher stress — opportunity to offer revised credit limits with conditions.

Demographic trend:

Defaults are slightly higher among younger customers (age 25–35) with university education, possibly due to unstable income patterns.

Policy implication:

Financial institutions can integrate this pipeline to automatically score customers each billing cycle using Databricks workflows.

# 7. Conclusion

This project demonstrates a scalable big data ML pipeline that predicts credit risk, segments customers, and provides actionable insights using Databricks.

Future Scope: Integrate streaming data and use deep learning for real-time predictions.
