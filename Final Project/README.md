# 📊 Holistic Data Preparer

## 🚀 Overview

Holistic Data Preparer is a complete end-to-end **data preprocessing and feature engineering project** built to transform raw data into a machine-learning-ready format.

This project demonstrates practical preprocessing workflows including:

- Data acquisition
- Data cleaning
- Missing value handling
- Outlier treatment
- Encoding
- Feature engineering
- Scaling
- Data transformations

---

## 🎯 Objectives

- Load data from multiple sources
- Analyze data quality
- Handle missing values using multiple techniques
- Detect and treat outliers
- Encode categorical variables
- Perform feature scaling and transformations
- Generate final cleaned and scaled datasets

---

## 📁 Dataset Sources

This project uses data from multiple formats:

- `customer_credit_risk.csv`
- `customer_metadata.json`
- `loan_history.db`

### 📂 Dataset Folder Structure

```bash
Dataset/
│
├── customer_credit_risk.csv
├── customer_metadata.json
└── loan_history.db
```

---

## 🛠️ Techniques Implemented

### 🔹 Missing Value Handling

- Complete Case Analysis
- Mean Imputation
- Most Frequent Imputation
- Missing Indicator
- Random Sample Imputation
- KNN Imputation
- MICE Imputation

---

### 🔹 Outlier Detection & Treatment

- Z-Score Method
- IQR Method
- Percentile Method
- Winsorization

---

### 🔹 Encoding Techniques

- Label Encoding
- Ordinal Encoding
- One Hot Encoding
- Binarization

---

### 🔹 Feature Scaling

- StandardScaler
- MinMaxScaler
- MaxAbsScaler
- RobustScaler
- Normalization

---

### 🔹 Data Transformations

- Log Transformation
- Square Root Transformation
- Reciprocal Transformation
- Box-Cox Transformation
- Yeo-Johnson Transformation

---

### 🔹 Feature Engineering

Created custom features such as:

- Debt-to-Income Ratio
- Spending-Income Ratio
- Monthly Transaction Metrics

---

## 📊 Best Methods Selected

After comparing multiple preprocessing techniques:

- ✅ **Best Numerical Imputation:** Mean Imputation
- ✅ **Best Categorical Imputation:** Most Frequent Imputation
- ✅ **Best Outlier Handling:** Winsorization
- ✅ **Best Encoding:** One Hot Encoding / Ordinal Encoding
- ✅ **Best Scaling Method:** StandardScaler

---

## 📂 Project Structure

```bash
Final Project/
│
├── Dataset/
│   ├── customer_credit_risk.csv
│   ├── customer_metadata.json
│   └── loan_history.db
│
├── holistic_data_preparer.ipynb
├── final_cleaned_dataset.csv
├── scaled_dataset.csv
├── data_quality_report.html
└── README.md
```

---

## 📈 Output Files

Generated files:

- `final_cleaned_dataset.csv`
- `scaled_dataset.csv`
- `data_quality_report.html`

---

## 🧠 Key Learnings

- Handling real-world messy datasets
- Comparing preprocessing methods
- Feature engineering workflow
- Preparing datasets for machine learning pipelines

---

## 🚀 Conclusion

This project successfully transforms raw customer credit data into a clean, structured, and machine-learning-ready dataset.

It demonstrates a holistic preprocessing workflow by evaluating multiple techniques and selecting the most effective methods for the dataset.

---

## 🙌 Author

**Herit Tanna**  
Data Science | Machine Learning | Data Analysis