# 🛍 Customer Purchase Propensity — Data Cleaning & Feature Engineering Pipeline

---

## 📌 Project Overview

This project presents a complete **end-to-end data preprocessing and feature engineering pipeline** for an e-commerce dataset.

The objective is to convert raw, multi-source data into a structured and analysis-ready format that can later be used for predicting customer purchase behavior using machine learning.

The entire workflow focuses on **data quality improvement, feature transformation, and dataset preparation**, rather than model building.

> 🎯 Goal: Predict customer purchase behavior (Binary Classification: 0 / 1)

---

## 📂 Data Sources

This project combines data from multiple structured sources:

- **Customer Data (CSV)** → demographic and profile information  
- **Transaction Data (JSON)** → purchase history and behavior  
- **Product Data (SQL / SQLite)** → product-level details  

All datasets are integrated using common identifiers such as `customer_id` and `product_id`.

---

## 🧭 Project Workflow

The project follows a structured 10-step data science pipeline:

---

### 1️⃣ Problem Understanding
- Defined business objective as a classification problem  
- Identified target variable: customer purchase behavior  
- Selected relevant features affecting customer decisions  

---

### 2️⃣ Data Collection & Integration
- Loaded data from CSV, JSON, and SQL sources  
- Standardized formats and data types  
- Merged datasets into a single analytical table  

---

### 3️⃣ Exploratory Data Analysis (EDA)
- Studied feature distributions  
- Identified skewness and anomalies  
- Analyzed relationships between variables and target  

---

### 4️⃣ Missing Data Treatment
- Applied multiple imputation strategies:
  - Mean/Mode Imputation  
  - KNN Imputation  
  - Iterative (MICE) Imputation  
- Used missing indicators to capture data absence patterns  

---

### 5️⃣ Outlier Treatment
- Z-score based detection  
- IQR-based filtering  
- Percentile capping  
- Winsorization for extreme values  

---

### 6️⃣ Feature Engineering (Time & Mixed Data)
- Converted date fields into datetime format  
- Created features like:
  - Customer tenure  
  - Days since last purchase  
- Cleaned inconsistent identifiers and mixed formats  

---

### 7️⃣ Encoding Categorical Variables
- Label Encoding for binary categories  
- One-Hot Encoding for nominal variables  
- Ordinal Encoding for ranked categories  
- Income segmentation using binning  

---

### 8️⃣ Feature Scaling
- StandardScaler  
- MinMaxScaler  
- MaxAbsScaler  
- RobustScaler (preferred for outlier-heavy data)  
- Normalization techniques  
- ColumnTransformer for hybrid scaling  

---

### 9️⃣ Feature Construction & Transformation
- Engineered behavioral features (purchase rate, spending patterns)  
- Applied mathematical transformations:
  - Log transformation  
  - Square root transformation  
  - Reciprocal transformation  
- Power transformation for distribution normalization  
- Created customer segmentation features  

---

### 🔟 Final Output Generation
- Exported processed dataset as `processed_customer_data.csv`  
- Final dataset fully cleaned and feature-engineered  
- Ready for machine learning modeling phase  

---

## 📊 Final Dataset Summary

- Total Records: ~1000+  
- Features: 45+ engineered variables  
- Missing Values: None (post-processing)  
- Fully encoded, scaled, and transformed dataset  

---

## 🧰 Tools & Technologies

- Python  
- Pandas, NumPy  
- Scikit-learn  
- SciPy  
- Matplotlib, Seaborn  
- SQLite3  
- JSON handling  

---

## 💡 Key Learnings

- Real-world datasets require multi-stage cleaning pipelines  
- Feature engineering significantly improves data usability  
- Multiple imputation and scaling techniques must be compared  
- Data preprocessing is the foundation of machine learning success  

---

## 🚀 Future Scope

- Machine learning model development  
- Feature importance analysis  
- Model performance comparison  
- Deployment using API or dashboard  
