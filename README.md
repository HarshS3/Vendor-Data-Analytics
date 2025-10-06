# Vendor Performance Analysis using Python and Power BI

## 📌 Overview
This project focuses on analyzing vendor performance based on sales data. It involves data ingestion, cleaning, exploratory data analysis (EDA), automation of summary generation, and dashboard development using Power BI. The objective is to help decision-makers identify underperforming vendors, optimize procurement strategies, and enhance vendor management.
The project concludes with a comprehensive report containing actionable insights.

## 📂 Project Structure
```
├── data/
│   ├── begin_inventory.csv
│   ├── end_inventory.csv
│   ├── purchases.csv
│   ├── purchase_prices.csv
│   ├── sales.csv
│   └── vendor_invoice.csv
├── Exploratory Data Analysis.ipynb
├── Vendor Performance Analysis.ipynb
├── get_vendor_summary.py
├── ingestion_db.py
├── vendor_performance.pbix
├── Vendor Performance Report.pdf
├── vendor_sales_summary.csv
├── requirements.txt
└── README.md
```

## 🛠️ Tech Stack
- **Languages**: Python (Pandas, Matplotlib, Seaborn), SQLite3
- **Tools**: Jupyter Notebook, Power BI, Excel
- **Other**: PDF Reporting, Logging

## 💡 Key Features
- Automated ingestion and cleaning of vendor sales data
- Detailed Exploratory Data Analysis (EDA) to identify trends and patterns
- Python scripts for automated vendor summary reports
- Interactive and visually rich dashboard built using Power BI
- Finalized insights compiled in a professional PDF report

 ## 🧩 Project Workflow

### 1. 🧠 Data Ingestion & Transformation (Script: `get_vendor_summary.py`)

### 2. 📊 Exploratory Data Analysis (EDA)

Performed initial EDA using Python:
- Checked for null values, outliers, and duplicates
- Grouped vendors by category and calculated metrics
- Used summary statistics to understand data distribution
- Optional visualizations: Bar charts, box plots, etc.

### 3. 📈 Vendor Performance Analysis
It answers following business questions:
- Identifying Brands that needs Promotional or Pricing Adjustments which exhibit lower sales performance but higher profit margins.
- Which vendors and brands demonstrate the highest sales performance?
- Which vendors contribute the most to toal purchase dollars?
- How much of total procurement is dependent on the top vendors?
- Does purchasing in bulk reduce the unit price, and what is the optimal purchase volume for cost savings?
- How much capital is locked in unsold inventory per vendor and which vendors contribute the most to it?

  ### 4. 📉 Power BI Dashboard



## 🚀 Setup and How to Run

1) Create a Python environment and install dependencies

Windows (cmd):

```
cd D:\Projects\VPDA
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

2) Ingest CSVs into SQLite

```
python ingestion_db.py
```

This reads all CSVs from `data/` and creates `inventory.db` with tables named after the files (e.g., `purchases`, `sales`, `vendor_invoice`, ...).

3) Build vendor summary table and write KPIs

```
python get_vendor_summary.py
```

This creates/updates the `vendor_sales_summary` table in `inventory.db` and logs to `logs/get_vendor_summary.log`. You can optionally export it from the analysis notebook.

4) Explore and visualize

- Open `Vendor Performance Analysis.ipynb` to explore KPIs and charts.
- Open `vendor_performance.pbix` in Power BI for the dashboard.

Notes
- Logs are written under `logs/` automatically.
- If CSVs are very large, consider chunked ingestion (future improvement).

## 📈 Outputs
- Vendor performance summary CSV
- Power BI Dashboard
- Final insights PDF report
