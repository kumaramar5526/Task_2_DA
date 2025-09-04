# EDA on Stores.csv

## Overview
This project performs **Exploratory Data Analysis (EDA)** on the provided dataset `Stores.csv`.  
The goal is to uncover meaningful business insights using **visualizations** and **statistical summaries**.

## Steps Performed
1. **Data Loading**
   - Loaded `Stores.csv` into a Pandas DataFrame.
   - Identified numeric and categorical columns.

2. **Data Quality Checks**
   - Checked dataset shape, data types, missing values, duplicate rows.
   - Saved column-wise summary (`dtype`, missing count, unique values).

3. **Descriptive Statistics**
   - `.describe()` for numeric & categorical columns.
   - Exported detailed summaries to CSV.

4. **Visualizations**
   - Missing values heatmap.
   - Histograms + Boxplots for numeric columns.
   - Correlation heatmap (for numeric variables).
   - Scatter matrix (if ≤6 numeric columns).
   - Barplots for top categories in categorical columns.

5. **Outlier & Skewness Analysis**
   - Calculated skewness for numeric columns.
   - Detected outliers using **IQR method**.
   - Logged insights in summary.

6. **Deliverables**
   - **EDA_Report.pdf** → Professional PDF report with plots and findings.
   - **EDA_Stores_notebook.ipynb** → Jupyter Notebook to reproduce the analysis.
   - **column_summary.csv, numeric_describe.csv, categorical_describe.csv** → Tabular summaries.
   - **short_summary.txt** → Quick text summary of dataset health & key stats.
   - **Stores_clean_shallow.csv** → Lightly cleaned dataset (duplicates dropped).

## Tools Used
- **Python**: pandas, numpy, matplotlib, seaborn
- **ReportLab**: for PDF generation
- **nbformat**: for reproducible Jupyter Notebook

## How to Run
```bash
pip install pandas numpy matplotlib seaborn reportlab nbformat
python EDA_Stores_notebook.py
