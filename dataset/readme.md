# 📊 Dataset Description – Customer Churn Prediction

## 📌 Overview
This dataset is used to build a **Customer Churn Prediction** model for a telecom company.  
The goal is to predict whether a customer will **churn (Yes/No)** based on their
demographic details, service usage, and billing information.

---

## 📂 Files Included
| File Name | Description |
|----------|-------------|
| `train.xlsx` | Training dataset containing customer features and churn label |
| `test.xlsx` | Testing dataset used for model validation |

---

## 🎯 Target Variable
- **Churn**
  - `Yes` → Customer has churned
  - `No` → Customer is retained

---

## 🧾 Feature Description

### 🧍 Customer Information
| Feature | Description |
|-------|-------------|
| `customerID` | Unique customer identifier |
| `gender` | Male / Female |
| `SeniorCitizen` | 1 = Senior citizen, 0 = Not a senior citizen |
| `Partner` | Whether customer has a partner |
| `Dependents` | Whether customer has dependents |

---

### 📞 Service Details
| Feature | Description |
|-------|-------------|
| `tenure` | Number of months customer has stayed |
| `PhoneService` | Whether phone service is active |
| `MultipleLines` | Whether customer has multiple phone lines |
| `InternetService` | Type of internet service (DSL, Fiber optic, None) |
| `OnlineSecurity` | Whether online security service is enabled |
| `OnlineBackup` | Whether online backup service is enabled |
| `DeviceProtection` | Whether device protection is enabled |
| `TechSupport` | Whether technical support is enabled |
| `StreamingTV` | Whether streaming TV service is enabled |
| `StreamingMovies` | Whether streaming movies service is enabled |

---

### 💳 Billing Information
| Feature | Description |
|-------|-------------|
| `Contract` | Contract duration (Month-to-month, One year, Two year) |
| `PaperlessBilling` | Whether paperless billing is enabled |
| `PaymentMethod` | Method of payment |
| `MonthlyCharges` | Monthly bill amount |
| `TotalCharges` | Total amount charged |

---

## ⚙️ Data Preprocessing Steps
- Removed duplicate records
- Converted `TotalCharges` from object to numeric
- Handled missing values
- Dropped `customerID` during modeling
- Applied **One-Hot Encoding** to categorical features
- Performed **correlation-based feature selection**

---

## 📊 Dataset Size
- **Rows:** 7,043  
- **Columns:** 21  

---

## 📚 Source
This dataset is based on a **telecom customer churn dataset** commonly used for
machine learning classification problems and academic practice.

---

## ⚠️ Note
This dataset is used **only for educational and learning purposes**.
