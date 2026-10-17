# Enterprise_Data_Reconciliation
Enterprise Data Reconciliation is a Python and SQLite project that processes 100,000 transaction logs, extracts transaction details with regular expressions, identifies customers with an active latest account status, and converts EUR transactions to USD using daily exchange rates.

## Project Overview

This project combines transaction logs, customer account history, and daily EUR-to-USD exchange rates to produce revenue summaries for a fictional FinTech company. It uses Python, pandas, SQLite, and Matplotlib/Seaborn.

## Objectives

- Extract transaction details from unstructured server logs.
- Exclude log entries marked `ERROR`.
- Identify each user’s most recent account status with a SQL window function.
- Keep transactions associated with users whose latest status is `Active`.
- Convert transaction amounts from euros to US dollars using daily exchange rates.
- Summarize revenue by month and identify the top five customers.
- Visualize the results.

## Project Files

- `Enterprise_Data_Reconciliation_Project.ipynb` — notebook containing the analysis.
- `server_logs.txt` — transaction log input.
- `daily_exchange_rates.csv` — daily exchange-rate input.
- `enterprise_database.db` — SQLite customer history database.
- `reconciled_transactions.csv` — transaction-level results.
- `monthly_revenue.csv` — monthly revenue summary.
- `top_5_customers.csv` — top-five customer summary

## Tools

- Python
- pandas
- SQLite (`sqlite3`)
- Regular expressions (`re`)
- Matplotlib
- Seaborn
- Jupyter Notebook

## How to Run

1. Clone or download this repository.
2. Install the required packages:

   ```bash
   pip install pandas matplotlib seaborn jupyter
