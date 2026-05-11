# 📉 Telecom Customer Churn Analysis using Python

An exploratory data analysis of a telecom company's customer dataset to understand churn behaviour, identify at-risk customer segments, and uncover the key factors that drive customers to leave the service.

---

## 📌 Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses. This project analyzes the **IBM Telco Customer Churn dataset** to answer 15 business questions around demographics, subscription types, charges, and churn patterns — helping businesses understand **who churns, why, and when**.

---

## 📂 Dataset

- **Source:** [Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **File used:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`
- **Size:** 7,043 customers × 21 attributes
- **Key columns:** `customerID`, `gender`, `SeniorCitizen`, `tenure`, `Contract`, `MonthlyCharges`, `TotalCharges`, `Churn`

---

## 🧹 Data Preparation

- Converted `TotalCharges` from object to numeric using `pd.to_numeric` with error coercion
- Checked for null values and data types across all 21 columns
- Identified and handled data gaps (e.g., no location data available in the dataset)

---

## 🔍 15 Business Questions Answered

| # | Question |
|---|---|
| 1 | How many customers are present in the dataset? |
| 2 | What is the distribution of gender among customers? |
| 3 | How does age (Senior vs Non-Senior) vary among customers? |
| 4 | What are the different locations customers belong to? |
| 5 | How long have customers been using the service on average? |
| 6 | What is the distribution of subscription/contract types? |
| 7 | What is the average monthly charge incurred by customers? |
| 8 | What is the range of total charges accumulated by customers? |
| 9 | How many customers have churned? |
| 10 | What is the overall churn rate? |
| 11 | How does churn vary across different genders? |
| 12 | Are there differences in churn based on customer age (Senior vs Non-Senior)? |
| 13 | Are customers from specific locations more likely to churn? |
| 14 | Does the subscription/contract type influence customer churn? |
| 15 | Is there any correlation between monthly charges and total charges? |

---

## 💡 Key Insights

- 📊 The dataset contains **7,043 unique customers**
- ⏱️ Customers have been using the service for an average of **32 months**
- 📉 The overall **churn rate is ~26.5%** — roughly 1 in 4 customers leaves
- 👫 Churn is **nearly equal across genders** — gender is not a major churn predictor
- 👴 **Senior Citizens churn more** proportionally than non-senior citizens
- 📋 Customers on **Month-to-Month contracts churn the most** — long-term contracts significantly improve retention
- 💳 There is a **positive correlation** between monthly charges and total charges, as expected

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core language |
| Pandas | Data loading, cleaning & grouping |
| NumPy | Numerical calculations & floor function |
| Google Colab | Development environment |

---

## 🚀 How to Run

### Option 1 — Open in Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

*(Replace with your actual Colab notebook link)*

### Option 2 — Run Locally
```bash
git clone https://github.com/anshu1516/Telecom-Customer-Churn-Analysis.git
cd Telecom-Customer-Churn-Analysis

pip install pandas numpy

jupyter notebook Case_Study_Retain_Customers.ipynb
```

> **Note:** Download `WA_Fn-UseC_-Telco-Customer-Churn.csv` from Kaggle and place it in the same directory before running.

---

## 👤 Author

**Anshu** — [GitHub](https://github.com/anshu1516)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
