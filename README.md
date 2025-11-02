# 📊 Telco Customer Churn Prediction

## 🧠 Project Overview
This project predicts **customer churn** — whether a customer is likely to discontinue the telecom service — using machine learning.  
By identifying potential churners early, telecom companies can **retain customers**, **reduce losses**, and **improve satisfaction**.

---

## 📁 Dataset Information
**Dataset:** Telco Customer Churn  
**Total Records:** 7,043  

### 🔑 Key Features
- **Demographics:** Gender, SeniorCitizen, Partner, Dependents  
- **Account Info:** Tenure, Contract, PaymentMethod, PaperlessBilling  
- **Service Usage:** InternetService, PhoneService, StreamingTV, StreamingMovies  
- **Financials:** MonthlyCharges, TotalCharges  
- **Target Variable:** `Churn` (Yes / No)

---

## ⚙️ Data Preprocessing
Steps performed before modeling:
1. **Handled missing values** — replaced missing `TotalCharges` with median value.  
2. **Encoded categorical features** — converted text categories to numeric values using Label Encoding.  
3. **Feature scaling** — standardized numerical columns for better model performance.  
4. **Train-Test Split** — 80% training, 20% testing data.

---

## 🔍 Exploratory Data Analysis (EDA)
Some major insights from data visualization:
- Average customer **tenure** = 32.37 months  
- Average **monthly charges** = ₹64.76  
- Most common **Internet Service** = Fiber optic (43.96%)  
- Top **Payment Method** = Electronic check  
- **Month-to-month** contracts have the highest churn rate  
- Long-term contracts (1 or 2 years) have lower churn probability  

---

## 🤖 Model Used
**Model:** Logistic Regression  
Chosen because it’s simple, interpretable, and effective for binary classification.

---

## 📈 Model Performance

| Metric | Score |
|--------|--------|
| **Accuracy** | ~0.8147 |
| **ROC-AUC Score** | 0.861 |

✅ **Interpretation:**  
The model performs well at distinguishing between churners and non-churners, with a strong ROC-AUC score.

---

## 💡 Key Insights
- Customers with **month-to-month contracts**, **higher monthly charges**, and **fiber optic service** are more likely to churn.  
- Customers on **long-term contracts** and **auto-payment methods** are less likely to churn.  
- Customers paying via **electronic check** churn more often — possibly due to higher manual effort or dissatisfaction.

---

## 📊 Power BI Dashboard
![Telco Customer Churn Dashboard](dashboard.png)

### Dashboard Highlights
- **Total Records:** 7,043  
- **Average Tenure:** 32.37 months  
- **Average Monthly Charges:** ₹64.76  
- **Most common Internet Service:** Fiber optic (43.96%)  
- **Top Payment Method:** Electronic Check  
- **Churn patterns:** Higher for month-to-month and electronic check customers  

🎯 The dashboard helps business teams visualize churn trends, compare services, and focus on at-risk customer groups.

---

## 🧰 Tools & Libraries
- **Python**
  - pandas  
  - numpy  
  - matplotlib / seaborn  
  - scikit-learn  
- **Power BI** – for dashboard visualization  
