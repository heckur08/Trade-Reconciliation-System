# 🧾 Trade Reconciliation System

This project simulates and audits a trade reconciliation pipeline — a core process in financial systems that validates consistency between executed and reported trades. It replicates real-world post-trade checks with data discrepancies, fuzzy field-level matching, and persistent storage using MySQL.

---

## 📌 Features

-  **Synthetic trade data generation** for both executed and reported trades
-  **Intentional discrepancies** added to simulate real-world reporting mismatches
-  **Fuzzy reconciliation logic** with customizable tolerance:
  -  Price difference ≤ 0.01%
  -  Quantity difference ≤ ±1 unit
  -  Timestamp difference ≤ ±1 second
-  Field-level mismatch tagging: Price, Quantity, Timestamp
-  MySQL integration for storing original trades and reconciled results
-  SQL-based reporting for summarizing mismatches per account or contract

---

## 📂 Project Structure
```
trade-reconciliation/
├── trade_reconciliation.ipynb       # Full notebook with code, outputs & markdown
├── executed_trades.csv              # Sample executed trades
├── reported_trades.csv              # Sample reported trades with injected errors
├── fuzzy_field_mismatches.csv       # Output: field-level mismatches
├── missing_trades.csv               # Output: missing trade reports
├── requirements.txt                 # List of Python dependencies
└── README.md                        # Project overview (this file)
```

---

## 🚀 How to Run

### 🔧 Requirements
Install the required libraries:

```bash
pip install -r requirements.txt
```
Make sure MySQL is running and a database named trade_db exists. Set your credentials in the notebook before running MySQL queries.

### ▶️ Steps
Load trade_reconciliation.ipynb in Jupyter Notebook

Follow the notebook steps:

Load data

Reconcile trades with tolerance

Tag mismatches

Push data to MySQL

Run SQL summaries

Optionally export results as CSV

## 💡 What You'll Learn
How to simulate data-driven financial problems

Performing tolerance-based comparison in Python

Handling floating-point discrepancies and timestamp drift

Integrating SQL with pandas for backend auditability

Building data pipelines ready for financial compliance reporting

## 🛠️ Tech Stack
Python 3.12+

Pandas, NumPy

MySQL, SQLAlchemy

Jupyter Notebook

## 📜 License
This project is licensed under the MIT License. Feel free to reuse, extend, or modify.

## 👤 Author
Anurag Singh
B.Tech, IIT Patna
📫 Reach me at: [anuragsingh133125@gmail.com]

Let me know if you'd like it personalized further with:
- A live project badge
- A "Used in Resume Projects" line
- GIF/visuals if you're hosting screenshots
