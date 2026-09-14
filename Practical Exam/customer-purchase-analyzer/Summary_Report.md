# Summary Report – Customer Purchase Behavior Analyzer

## Theory

This project combines data from three different sources — a CSV file (customers), a JSON file
(sales transactions), and a SQL file (product catalog) — into one clean dataset that can be used
for further analysis or machine learning.

- **Missing value handling** was done using `SimpleImputer`. Numeric columns were filled with the
  mean, and categorical columns were filled with the most frequent value, since this is a simple
  and commonly used approach that doesn't distort the data too much.
- **Outlier detection** was done using two methods: the **Z-score** method (flags values more than
  3 standard deviations from the mean, works best on normal-looking data) and the **IQR method**
  (flags values outside 1.5×IQR from the quartiles, works better for skewed data). Since purchase
  amounts are usually right-skewed (a few big spenders), the IQR method was considered more
  reliable here. Outliers were **capped using Winsorization** rather than deleted, so no real
  transaction data is lost.
- **Encoding**: Label Encoding was used for gender (few categories), One-Hot Encoding was used for
  payment type (no natural order), and Ordinal Encoding was used for the spending group
  (Low < Medium < High has a real order).
- **Scaling**: StandardScaler centers data around 0 with unit variance, while MinMaxScaler squashes
  values into a 0–1 range. Both were compared on the `amount` column.
- **Feature Engineering**: new customer-level features were built — average monthly spend,
  purchase frequency, days since last purchase, and category-wise total spend — because these
  describe *behavior* better than the raw transaction rows do.

## Observations

- The raw data provided (`users.csv`, `sales.json`, `inventory.sql`) was already fairly clean:
  no missing values, no negative prices/amounts, and no invalid date formats were found.
- A small number of outlier transactions were found in the `amount` column using the IQR method;
  these were capped (winsorized) instead of removed.
- After merging, the final dataset has **200 rows** (one per customer) and **23 columns**,
  combining demographic info with the newly engineered purchase-behavior features.
- The final cleaned dataset was saved as `final_cleaned_dataset.csv`.

## Deliverables

- `main.ipynb` – full notebook with all steps
- `final_cleaned_dataset.csv` – final dataset
- `README.md` – setup and run instructions
