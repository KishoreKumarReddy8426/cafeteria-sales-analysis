# ☕ Cafeteria Sales Data Analysis

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4c72b0)](https://seaborn.pydata.org/)

A practical **Python data-analysis project** that transforms one year of cafeteria transaction data into sales trends, product insights, data-quality findings, and business recommendations.

> **Raw Data → Data Quality Checks → Cleaning → Feature Creation → EDA → Visualization → Business Insights**

---

## 📌 Project Overview

This project demonstrates an end-to-end exploratory data analysis workflow using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

The analysis covers:

- Data-quality inspection
- Missing-value handling
- Invalid-value removal
- Duplicate removal
- Data-type conversion
- Feature creation
- Monthly revenue analysis
- Product performance
- Day-of-week sales analysis
- Descriptive statistics
- Correlation analysis
- Business recommendations

---

## 🎯 Business Questions

The project is designed to answer:

1. Which month generates the highest and lowest revenue?
2. Which products sell the highest number of units?
3. Which day of the week generates the most revenue?
4. What are the main characteristics of the transaction data?
5. What relationships exist between Quantity, Price Per Unit, and Total Price?
6. What data-quality issues exist in the raw dataset?
7. What operational actions can be considered from the observed patterns?

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| Dataset | Cafeteria Sales Data |
| File | `data/Cafeteria.csv` |
| Period | January 2023 – December 2023 |
| Transactions | 10,000 |
| Granularity | Transaction-level sales data |

### Revenue Formula

```text
Total Price = Quantity × Price Per Unit
```

---

## 🧹 Data Cleaning

The analysis script performs:

- Dataset structure and data-type inspection
- Missing-value reporting
- Removal of rows missing critical transaction fields
- Removal of `UNKNOWN` and `ERROR` records
- Transaction-date conversion to datetime
- Quantity and unit-price conversion to numeric
- Removal of records that remain invalid
- Duplicate removal
- Creation of the `Total Price` metric

---

## 🔍 Exploratory Data Analysis

### Descriptive Statistics

The project calculates statistics for:

- Quantity
- Price Per Unit
- Total Price

Including mean, standard deviation, minimum, maximum, and quartiles.

### Monthly Revenue

Transactions are grouped by month to compare total revenue throughout the year.

### Product Performance

Products are ranked by total quantity sold to identify high-volume items.

### Day-of-Week Analysis

Revenue is grouped by day of week to identify higher-revenue sales days.

### Correlation Analysis

The project examines relationships between:

- Quantity
- Price Per Unit
- Total Price

> **Important analytical note:** `Total Price` is mathematically derived from `Quantity × Price Per Unit`. Therefore, its strong correlation with those variables is expected and should not be interpreted as evidence of an independent causal relationship.

---

## 📈 Visualizations

Running `cafeteria_analysis.py` generates:

| Visualization | Purpose |
|---|---|
| Correlation Heatmap | Examines relationships among numerical sales variables |
| Monthly Sales Bar Chart | Compares revenue across months |
| Top Selling Items Bar Chart | Shows the top 10 products by quantity sold |
| Peak Sales by Day | Compares revenue across days of the week |

---

## 💡 Current Findings

Based on the current dataset and analysis:

- **March** has the highest reported monthly revenue: **₹85,420**
- **August** has the lowest reported monthly revenue: **₹61,280**
- **Coffee** is the highest-selling product by quantity
- The day-of-week analysis identifies the highest-revenue sales day from the cleaned transaction data
- The strong Quantity–Total Price relationship is expected because Total Price is derived from those variables

These are descriptive findings from this dataset, not forecasts or causal conclusions.

---

## 🏪 Business Recommendations

### 📦 Inventory Planning
Use product-level sales volume to prioritize inventory for consistently high-demand items.

### 🎁 Product Bundling
Test bundles that combine high-demand products with lower-performing items.

### 📅 Promotional Planning
Investigate lower-revenue periods for targeted promotions and demand-generation campaigns.

### 👥 Staffing
Use day-of-week revenue patterns as one input when planning staffing requirements.

### ✅ Data Quality
Introduce validation rules during data entry to reduce missing, invalid, and inconsistent records.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **Python** | Analysis workflow and scripting |
| **Pandas** | Data cleaning, transformation, grouping, and analysis |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |

---

## 🧠 Skills Demonstrated

- Python programming
- Pandas
- NumPy
- Data cleaning
- Data validation
- Data wrangling
- Exploratory Data Analysis (EDA)
- Descriptive statistics
- GroupBy analysis
- Feature creation
- Correlation analysis
- Data visualization
- Business insight generation
- Data-driven recommendations

---

## 📁 Project Structure

The repository files verified while preparing this README are:

```text
cafeteria-sales-analysis/
│
├── data/
│   └── Cafeteria.csv
│
├── cafeteria_analysis.py
├── requirements.txt
├── Requirements_Document.pdf
└── README.md
```

### Important path note

The dataset is stored at:

```text
data/Cafeteria.csv
```

The current Python script uses:

```python
pd.read_csv("Cafeteria.csv")
```

So the script's data path should be aligned with the repository structure before running it from a fresh clone.

---

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KishoreKumarReddy8426/cafeteria-sales-analysis.git
cd cafeteria-sales-analysis
```

### 2. Install dependencies

The repository includes `requirements.txt`.

```bash
pip install -r requirements.txt
```

### 3. Run the analysis

```bash
python cafeteria_analysis.py
```

The script prints data-quality reports, descriptive statistics, correlation results, monthly revenue, top-selling products, and day-of-week analysis, while displaying the generated visualizations.

---

## 🚀 Future Improvements

- Align the script's dataset path with `data/Cafeteria.csv`
- Add a dedicated EDA notebook
- Add stronger statistical analysis and hypothesis testing
- Add additional business KPIs
- Build an interactive Streamlit dashboard
- Create Tableau and Power BI versions
- Add time-series sales forecasting
- Add customer segmentation when customer-level identifiers are available
- Add automated tests for data-quality rules
- Automate report generation

---

## 👨‍💻 About the Author

### Kishore Kumar Reddy

**Tableau Developer | Data Analyst | Python | SQL | Power BI**

Focused on building practical analytics projects that combine **data preparation, exploratory analysis, visualization, business intelligence, and machine learning**.

This project represents a step toward stronger Python-based data-analysis and data-science capabilities.

🔗 **GitHub:** [KishoreKumarReddy8426](https://github.com/KishoreKumarReddy8426)

---

## ⭐ Project Status

**Status:** Completed Python EDA project

**Focus:** Data cleaning, exploratory analysis, visualization, and business insights

**Next stage:** Expand the project with stronger statistical analysis, interactive dashboards, and machine-learning use cases.
