# 🧹 Data Cleanser Project

## 📌 Project Overview

This project focuses on cleaning a healthcare dataset by handling missing values and outliers using different data preprocessing techniques. The cleaned dataset becomes more reliable and suitable for data analysis and machine learning.

---

# 📂 Dataset

**Dataset Name:** `data_cleanser_dataset.csv`

The dataset contains patient health records with the following features:

- patient_id
- age
- gender
- region
- bmi
- blood_pressure
- cholesterol
- glucose
- disease_risk

---

# 🎯 Project Objectives

- Identify missing values in the dataset.
- Apply different missing value imputation techniques.
- Detect and handle outliers.
- Compare the dataset before and after cleaning.
- Generate a final cleaned dataset.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- SciPy
- Jupyter Notebook

---

# 📌 Part A: Handling Missing Values

The following missing value techniques were applied:

### ✅ Missing Value Analysis

- Checked missing values
- Calculated missing percentage
- Created missing value summary report

### ✅ Imputation Techniques

- Mean Imputation
- Most Frequent Imputation
- Random Sample Imputation
- Missing Indicator
- KNN Imputation
- MICE (Multiple Imputation by Chained Equations)

---

# 📌 Part B: Handling Outliers

The following outlier handling techniques were applied:

- Z-Score Method
- IQR Method
- Percentile Capping
- Winsorization

The dataset statistics and shape were compared before and after outlier treatment.

---

# 📌 Part C: Final Clean Dataset

The final cleaned dataset was created after:

- Handling missing values
- Treating outliers

The cleaned dataset was saved as:

```
Final_Clean_Dataset.csv
```

---

# 📊 Results

- Missing values were successfully handled.
- Outliers were reduced using Winsorization.
- Data quality and consistency improved.
- The dataset is now suitable for machine learning and data analysis.

---

# 📁 Project Files

```
Data_Cleanser_Project/
│
├── data_cleanser_dataset.csv
├── Final_Clean_Dataset.csv
├── Data_Cleanser_Project.ipynb
├── README.md
```

---

# 🚀 How to Run

1. Install the required libraries.

```
pip install pandas numpy scikit-learn scipy
```

2. Open the Jupyter Notebook.

3. Run all cells from top to bottom.

4. The cleaned dataset will be generated automatically.

---

# 📌 Conclusion

This project demonstrates the complete data cleaning process by handling missing values and outliers using multiple preprocessing techniques. The final cleaned dataset is more accurate, consistent, and ready for further analysis and machine learning applications.

# 📌 Video Explanation Link : 

https://drive.google.com/file/d/1l_vupDFYL2bub26xymGisZFJRvpCmZ9I/view?usp=sharing