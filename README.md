# 📉 Customer Churn Prediction using Logistic Regression (with Streamlit App)

This project predicts whether a customer will churn (leave the service) using a **Logistic Regression model**. It includes a user-friendly **Streamlit web interface** and provides helpful **churn prevention and retention tips** based on prediction results.

---

## 🧠 Objective

To build a classification model that predicts customer churn based on demographic and service-related features and deploy it using a Streamlit-based interface.

---

## 📊 Dataset Features

- Gender
- Senior Citizen
- Partner / Dependents
- Tenure
- PhoneService / MultipleLines
- Contract type
- Total Charges
- Churn (target variable)

---

## 🔍 Steps Followed

### ✅ Step 1: Importing Libraries
- pandas, numpy, sklearn, pickle
- Streamlit for web app interface

### ✅ Step 2: Load Dataset
- Data loaded from `7 churn.csv`

### ✅ Step 3: Data Preprocessing
- Selected important columns
- Label Encoding for binary/categorical features
- Train-test split
- Feature scaling using `StandardScaler`

### ✅ Step 4: Model Training
- Trained a **Logistic Regression** model
- Evaluated using **accuracy score**
- Saved model using `pickle` as `7 logistic_model.pkl`

---

## 💻 Streamlit Web App Features

- UI for selecting customer info (gender, senior citizen, partner, tenure, etc.)
- On clicking **“Predict churn or not”**, the app shows:
  - `Churn` or `Not Churn`
  - 10 useful tips depending on the result

### ✅ Libraries Used
```python
import streamlit as st
import pandas as pd
import numpy as np
import pickle
from sklearn.preprocessing import LabelEncoder, StandardScaler


Output Example
🔴 If customer is predicted to Churn:

Displays 10 Churn Prevention Tips (like personalized offers, engagement monitoring)

🟢 If customer is Not Churning:

Displays 10 Retention Tips (like loyalty programs, appreciation)

 Model Result
Logistic Regression Accuracy: ✅ (You can update with actual score like ~80–85%)

Real-time prediction with live user inputs

Simple yet effective classifier for business decisions

🚀 Future Improvements
Add more models (e.g., Random Forest, XGBoost)

Improve UI design of Streamlit app

Save prediction logs

Integrate with a database or dashboard

🔗 Project Links
🧑‍💻 GitHub: github.com/Vivek0980

📘 Notebook & Model: Coming Soon

🌐 Web App: Deploy on Streamlit Cloud or Render

