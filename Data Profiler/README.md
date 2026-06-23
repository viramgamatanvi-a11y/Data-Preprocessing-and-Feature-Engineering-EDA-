# 🏠 House Price Prediction - Data Analysis Project

## 📌 Project Overview

This project focuses on analyzing a House Price Prediction dataset using Python. The goal is to understand the data, perform data cleaning, exploratory data analysis (EDA), and generate an automated profiling report.

---

## 🎯 Objectives

* Load data from multiple sources
* Understand the dataset structure
* Clean and preprocess the data
* Perform Exploratory Data Analysis (EDA)
* Analyze relationships between variables
* Generate an automated profiling report

---

# 📂 Dataset Sources

The dataset was accessed from multiple sources:

* CSV File
* JSON File
* SQLite Database
* REST API

---

# 🛠️ Libraries Used

```python
pandas
numpy
matplotlib
seaborn
sqlite3
requests
ydata_profiling
```

---

# 📊 Project Workflow

## Part A: Fundamentals

The project begins with understanding:

* Data Analysis
* Data Science Project Lifecycle
* Machine Learning Problem Framing
* Tensors and their applications

---

## Part B: Data Acquisition

Data was collected from different sources:

### CSV File

* Loaded using Pandas

### JSON File

* Parsed using Pandas

### SQL Database

* Connected using SQLite

### API Data

* Fetched using Requests library

---

## Part C: Data Understanding & Cleaning

The following preprocessing steps were performed:

* Viewed first and last records
* Checked dataset shape
* Examined data types
* Converted categorical columns
* Generated statistical summary
* Checked duplicate records
* Identified missing values
* Calculated missing value percentages
* Filled missing values using median
* Separated numerical and categorical features

---

## Part D: Exploratory Data Analysis (EDA)

### Univariate Analysis

#### Numerical Features

* Histogram
* KDE Plot
* Box Plot
* Skewness
* Kurtosis

#### Categorical Features

* Value Counts
* Unique Values
* Count Plot
* Pie Chart

---

### Bivariate Analysis

#### Numerical vs Numerical

* Correlation Analysis
* Scatter Plot
* Regression Plot

#### Numerical vs Categorical

* GroupBy Analysis
* Violin Plot
* Bar Plot
* Box Plot

#### Categorical vs Categorical

Not performed because the dataset contains only one categorical feature (`ocean_proximity`).

---

### Multivariate Analysis

* Correlation Heatmap
* Pair Plot
* Scatter Plot with Hue and Size
* FacetGrid Visualization

---

## Part E: Data Profiling

Automated EDA report generated using:

```python
ydata_profiling
```

Generated Outputs:

* Interactive HTML Report
* Notebook Embedded Report

---

# 📈 Key Insights

* Median Income shows a strong relationship with House Value.
* Population distribution is right-skewed.
* Ocean proximity impacts house prices.
* Several numerical features are correlated with the target variable.
* Missing values were successfully handled before analysis.

---

# 🚀 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQLite
* Requests
* YData Profiling
* Jupyter Notebook

---

# 📄 Output

The project generates:

* Cleaned Dataset Analysis
* Visualizations and Insights
* Automated EDA Report (HTML)
* Data Profiling Report

---

## 👩‍💻 Author

**Tanvi**

House Price Prediction Data Analysis Project
