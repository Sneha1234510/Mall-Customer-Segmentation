# Task 1 Report: Data Cleaning and Preprocessing

## 1. Objective
The objective is to prepare the Mall Customer Segmentation dataset for analysis by checking missing values, duplicate records, inconsistent text, column names, and data types.

## 2. Dataset description
The original Kaggle dataset is commonly distributed as `Mall_Customers.csv`. It contains 200 customer records and five fields: CustomerID, Gender, Age, Annual Income (k$), and Spending Score (1-100).

**Source:** https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python

## 3. Tools used
- Python
- pandas
- Jupyter Notebook

## 4. Preprocessing methodology
1. Load the CSV file into a pandas DataFrame.
2. Inspect shape, column names, data types, missing values, and duplicate rows.
3. Standardize column names to lowercase with underscores.
4. Remove extra spaces and standardize gender labels.
5. Convert numeric fields to numeric data types.
6. Remove exact duplicate rows.
7. Fill numeric missing values with the median and categorical missing values with the mode.
8. Remove rows that still have no customer identifier.
9. Export the cleaned dataset and a cleaning summary.

## 5. Deliverables
- `src/clean_data.py` — reusable cleaning script.
- `notebooks/task1_data_cleaning.ipynb` — step-by-step notebook.
- `data/mall_customers_sample.csv` — 10-row demonstration input.
- `data/mall_customers_clean_sample.csv` — cleaned demonstration output.

## 6. Results and limitations
The included CSVs are only a 10-row demonstration sample because the full Kaggle file was not bundled. Therefore, no full-dataset cleaning counts are claimed here. Download the original 200-row CSV and run the script to generate the actual cleaned dataset and actual summary.

## 7. Conclusion
Data cleaning improves consistency and reliability before analysis. This project provides a repeatable workflow for checking and handling missing values, duplicates, text inconsistencies, and data types.
