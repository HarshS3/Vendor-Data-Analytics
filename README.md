# Vendor Performance Analysis using Python and Power BI

## 📌 Overview
This project focuses on analyzing vendor performance based on sales data. It involves data ingestion, cleaning, exploratory data analysis (EDA), automation of summary generation, and dashboard development using Power BI. The objective is to help decision-makers identify underperforming vendors, optimize procurement strategies, and enhance vendor management.
The project concludes with a comprehensive report containing actionable insights.

## 📂 Project Structure
```
├── data/
│   └── vendor_sales_summary.csv
├── notebooks/
│   ├── Exploratory Data Analysis.ipynb
│   └── Vendor Performance Analysis.ipynb
├── scripts/
│   ├── get_vendor_summary.py
│   └── ingestion_db.py
├── dashboard/
│   └── vendor_performance.pbix
├── reports/
│   └── Vendor Performance Report.pdf
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



## 🚀 How to Run
1. Clone the repository
2. Open Jupyter Notebook and run EDA and analysis notebook
3. Use `get_vendor_summary.py` to generate vendor summary from data
4. Open `.pbix` file in Power BI for dashboard view
5. Review the final report in `/reports`

## 📈 Outputs
- Vendor performance summary CSV
- Power BI Dashboard
- Final insights PDF report
