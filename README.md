# 📊 Customer Churn Analysis & Prediction Dashboard

## 🔍 Overview

This project presents an end-to-end **Customer Churn Analysis and Prediction System** built using **SQL Server, Power BI, and Machine Learning (Random Forest)**.

It combines **data engineering, business intelligence, and predictive analytics** to not only understand historical churn patterns but also identify customers who are likely to churn in the future.

The solution is designed to support **data-driven decision-making**, enabling businesses to take proactive steps to improve customer retention.

---

## 🎯 Objectives

* Build a complete **ETL pipeline** using SQL Server
* Perform **data cleaning and exploratory analysis**
* Develop an **interactive Power BI dashboard**
* Train a **machine learning model** to predict churn
* Deliver **actionable insights** for marketing and retention strategies

---

## 🛠️ Tech Stack

* **Database:** Microsoft SQL Server
* **Visualization:** Power BI
* **Programming:** Python (Jupyter Notebook)
* **Machine Learning:** Random Forest Classifier
* **Data Source:** Telecom Customer Churn Dataset

---

## ⚙️ Project Workflow

### 1. Data Engineering (ETL – SQL Server)

* Created database: `dbor_churn`
* Imported raw data into staging table: `STG_churn`
* Cleaned missing values and standardized fields
* Built production table: `prod_churn`
* Created analytical views:

  * `VW_churn_data`
  * `VW_join_data`

---

### 2. Data Analysis (SQL)

* Performed distribution analysis on:

  * Gender, contract type, customer status
  * State and internet service type
* Identified missing values and inconsistencies
* Generated percentage-based insights using SQL queries

---

### 3. Data Modeling (Power BI)

* Imported cleaned dataset from SQL Server
* Created calculated columns:

  * Churn indicator (`J_status`)
  * Monthly charge categories
* Built supporting dimension tables:

  * Age groups
  * Tenure groups

---

### 4. Key Measures (DAX)

* **Total Customers**
* **New Joiners**
* **Total Churn**
* **Churn Rate**

[
\text{Churn Rate} = \frac{\text{Total Churn}}{\text{Total Customers}}
]

---

### 5. Dashboard Development

#### 📌 Executive Summary Page

* KPI Cards (Customers, Churn, Joiners, Churn Rate)
* Demographics (Gender, Age Group)
* Account Information (Contract, Payment Method, Tenure)
* Geographic Analysis (Top states by churn)
* Service-level churn insights
* Interactive slicers and tooltips

#### 📌 Churn Prediction Page

* Predicted churners overview
* Customer segmentation by:

  * Gender
  * Age group
  * Contract type
  * Payment method
  * Geography
* Interactive drill-down analysis

---

## 🤖 Machine Learning Model

### Model Used: Random Forest Classifier

**Why Random Forest?**

* Handles categorical and numerical data well
* Reduces overfitting through ensemble learning
* Provides feature importance for interpretability

---

### Model Pipeline

* Data preprocessing:

  * Removed irrelevant columns
  * Encoded categorical variables
* Train-test split: **80% / 20%**
* Model training with **100 trees**
* Evaluation using:

  * Confusion Matrix
  * Classification Report

---

### 📈 Model Performance

| Metric    | Stayed (0) | Churned (1) |
| --------- | ---------- | ----------- |
| Precision | 86%        | 78%         |
| Recall    | 92%        | 65%         |
| F1 Score  | 89%        | 71%         |

* **Overall Accuracy:** 84%
* Model performs better on non-churners due to class imbalance

---

### 🔮 Prediction Results

* Applied model on new customer data (`VW_join_data`)
* Generated predictions and exported as CSV
* Identified **378 potential churners**

---

## 📊 Key Insights

* Higher churn observed among **customers aged 50+**
* **Competitor offers and better devices** are major churn drivers
* Certain services show strong churn patterns:

  * Non-subscribers → higher churn (e.g., online security)
  * Subscribers → higher churn (e.g., unlimited data)
* Geographic churn patterns remain relatively stable

---

## 📤 Output

* ✔️ Fully interactive **Power BI Dashboard** 
* ✔️ Cleaned and structured **SQL database**
* ✔️ Trained **machine learning model**
* ✔️ CSV file with **predicted churn customers**
* ✔️ Actionable business insights for retention strategies
<img width="2302" height="1322" alt="Image" src="https://github.com/user-attachments/assets/f8c520bd-1817-4f97-8f0d-3ce9c44810a0" />
---

## 🎥 Sample Demo Video



## 📌 Project Highlights

* End-to-end implementation (ETL → BI → ML)
* Business-focused insights, not just technical outputs
* Clean and intuitive dashboard design
* Scalable pipeline for real-world datasets

---

## 🚀 Future Improvements

* Handle class imbalance using SMOTE or class weighting
* Deploy model as an API for real-time predictions
* Automate data pipeline (ETL scheduling)
* Integrate directly with Power BI for live predictions

---

## 📚 Key Concepts

* Customer Churn Analysis
* ETL Pipeline
* Data Visualization
* Classification Metrics
* Predictive Analytics
* Feature Importance

---


