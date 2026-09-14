# Customer Purchase Behavior Analyzer

This project was made for the "Customer Purchase Behavior Analyzer" practical exam.
The goal is to load customer, sales and product data from 3 different file formats,
clean the data, create some new features, and save one final combined dataset.

## Files in this repo

- `main.ipynb` – the main Jupyter notebook with all the steps (loading, cleaning, outlier handling, transformation, scaling, feature construction, final dataset).
- `final_cleaned_dataset.csv` – the final cleaned and feature-engineered dataset (one row per customer).
- `Summary_Report.md` – short report explaining the theory used and what was observed in the data.
- `data/` – the original raw input files given for the project:
  - `users.csv`
  - `sales.json`
  - `inventory.sql`

## How to run

1. Install the required libraries:
   ```
   pip install pandas numpy scikit-learn scipy matplotlib
   ```
2. Open `main.ipynb` in Jupyter Notebook / Jupyter Lab / VS Code.
3. Run all the cells from top to bottom.
4. The final output `final_cleaned_dataset.csv` will be regenerated in the same folder.

## What the notebook does (step by step)

1. **Data Loading** – reads `users.csv` with pandas, `sales.json` with the json module, and `inventory.sql` by running the SQL script inside an in-memory SQLite database.
2. **Data Cleaning** – checks for missing values, duplicate rows, negative prices/amounts, and invalid dates. Uses `SimpleImputer` for numeric/categorical missing values and `KNNImputer` as an optional enhancement.
3. **Outlier Handling** – detects outliers in the `amount` column using both the Z-score method and the IQR method, and treats them using Winsorization.
4. **Data Transformation** – splits dates into day/month/year, does Label Encoding, One-Hot Encoding and Ordinal Encoding, bins customers into spending groups (Low/Medium/High), and applies log/sqrt transforms.
5. **Feature Scaling** – compares `StandardScaler` and `MinMaxScaler` on the amount column.
6. **Feature Construction** – builds new customer-level features: average monthly spend, purchase frequency, days since last purchase, and category-wise total expenditure.
7. **Final Dataset** – merges everything into one table and prints a before/after report (row counts, missing values, outlier counts, number of new features).
8. **Bonus** – a lightweight manual EDA summary (shape, dtypes, missing values, describe()) instead of a full profiling library, to keep things simple.

## Notes

- The raw data provided for this project was already fairly clean (no missing values or negative
  numbers were actually found), so the cleaning steps mostly print "0 issues found" — but the code
  is written so it will handle those issues if they show up in a different/updated dataset.
