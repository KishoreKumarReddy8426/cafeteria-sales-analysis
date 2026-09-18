# ☕ Cafeteria Sales Data Analysis

> **A practical Python data-analysis project focused on data cleaning, exploratory analysis, visualization, and business insights from one year of cafeteria transaction data.**

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4c72b0)

## 📌 Project Overview

This project demonstrates an end-to-end **exploratory data analysis (EDA) workflow using Python and Pandas** on one year of cafeteria sales transactions.

The objective is to transform raw transaction data into reliable, interpretable insights by:

- Inspecting dataset quality
- Handling missing and invalid values
- Removing duplicate records
- Converting and validating data types
- Creating calculated business metrics
- Analyzing sales trends
- Identifying top-performing products
- Examining sales by day of week
- Visualizing important patterns
- Translating analysis into business recommendations

### Analysis Workflow

**Raw Data → Data Quality Checks → Data Cleaning → Feature Creation → EDA → Visualization → Business Insights**

---

## 🎯 Business Questions

The analysis is designed to answer questions such as:

1. How does revenue change across months?
2. Which products sell the highest number of units?
3. Which days of the week generate the most revenue?
4. What does the distribution of quantity and price look like?
5. What relationships exist between the numerical sales variables?
6. What data-quality problems exist in the raw dataset?
7. What actions could a cafeteria take based on the observed patterns?

---

## 📊 Dataset

| Attribute | Details |
|---|---|
| Dataset | Cafeteria Sales Data |
| Source file | `Cafeteria.csv` |
| Period | January 2023 – December 2023 |
| Transactions | 10,000 |
| Granularity | Transaction-level sales data |

### Core Fields Used

The analysis uses fields including:

- Transaction Date
- Item
- Quantity
- Price Per Unit

A derived metric is created during analysis:

```text
Total Price = Quantity × Price Per Unit
```

---

## 🧹 Data Cleaning & Preparation

The analysis script performs several data-quality and preparation steps:

- Inspects the dataset structure
- Reports missing values
- Removes records missing critical transaction fields
- Removes rows containing `UNKNOWN` or `ERROR`
- Converts transaction dates to datetime
- Converts quantity and unit price to numeric values
- Removes records that remain invalid after conversion
- Removes duplicate records
- Creates the `Total Price` metric

This makes the dataset more suitable for downstream analysis and visualization.

---

## 🔍 Exploratory Data Analysis

### 1. Descriptive Statistics

The project calculates summary statistics for:

- Quantity
- Price Per Unit
- Total Price

The analysis includes measures such as mean, standard deviation, minimum, maximum, and quartiles.

### 2. Monthly Revenue Analysis

Transactions are grouped by month to identify changes in total revenue throughout the year.

### 3. Product Performance

Products are ranked by total quantity sold to identify the highest-volume items.

### 4. Day-of-Week Analysis

Transactions are grouped by day of week and ordered by total revenue to identify higher-revenue days.

### 5. Correlation Analysis

The project calculates correlations between:

- Quantity
- Price Per Unit
- Total Price

> **Important analytical note:** `Total Price` is mathematically derived from `Quantity × Price Per Unit`. Therefore, a strong correlation between these variables is expected and should not be interpreted as evidence of an independent causal relationship.

---

## 📈 Visualizations

Running `cafeteria_analysis.py` generates:

| Visualization | Purpose |
|---|---|
| Correlation Heatmap | Examines relationships among numerical sales variables |
| Monthly Sales Bar Chart | Compares revenue across months |
| Top Selling Items Bar Chart | Shows the top 10 products by quantity sold |
| Peak Sales by Day | Compares revenue across days of the week |

The visualizations are generated programmatically with **Matplotlib and Seaborn**.

---

## 💡 Current Findings

Based on the current dataset and analysis:

- **March** has the highest reported monthly revenue: **₹85,420**
- **August** has the lowest reported monthly revenue: **₹61,280**
- **Coffee** is the highest-selling product by quantity
- The day-of-week analysis identifies the highest-revenue sales day from the cleaned transaction data
- The strong relationship between Quantity and Total Price is expected because Total Price is derived from those variables

These findings are descriptive observations from the available dataset and should not be treated as forecasts.

---

## 🏪 Business Recommendations

### Inventory Planning
Use product-level sales volume to prioritize inventory for consistently high-demand items.

### Promotional Planning
Investigate lower-revenue months for targeted promotions and demand-generation campaigns.

### Staffing
Use day-of-week revenue patterns as one input when planning staffing requirements.

### Product Bundling
Explore bundles that combine high-demand products with lower-performing items.

### Data Quality Controls
Introduce validation rules at the point of data entry to reduce missing, invalid, and inconsistent records.

---

## 🛠️ Tech Stack

| Technology | Usage |
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

## 📁 Verified Project Files

The README documents the files currently verified in the repository:

```text
cafeteria-sales-analysis/
├── Cafeteria.csv
├── cafeteria_analysis.py
├── README.md
└── Requirements_Document.pdf
```

> **Note:** The analysis script currently reads `Cafeteria.csv` from the repository root using `pd.read_csv("Cafeteria.csv")`. Keeping the README and code paths consistent prevents setup errors.

---

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KishoreKumarReddy8426/cafeteria-sales-analysis.git
cd cafeteria-sales-analysis
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Run the analysis

```bash
python cafeteria_analysis.py
```

The script prints data-quality reports, descriptive statistics, correlation results, monthly revenue, top-selling products, and day-of-week sales analysis. It also displays the generated visualizations.

---

## 🔮 Future Improvements

The next iteration of this project could include:

- Add a dedicated `requirements.txt`
- Save and version visualization outputs
- Add a reusable data-cleaning pipeline
- Add additional business KPIs
- Build an interactive Streamlit dashboard
- Create Tableau / Power BI versions
- Add time-series sales forecasting
- Add customer segmentation when customer-level identifiers are available
- Add statistical hypothesis testing
- Add automated tests for data-quality rules
- Add automated report generation

---

## 👨‍💻 About the Author

### Kishore Kumar Reddy

**Tableau Developer | Data Analyst | Python | SQL | Power BI**

I am focused on building practical analytics projects that combine **data preparation, exploratory analysis, visualization, and business intelligence**.

This project represents a step toward developing stronger Python-based data-analysis and data-science capabilities.

🔗 **GitHub:** [KishoreKumarReddy8426](https://github.com/KishoreKumarReddy8426)

---

## ⭐ Why This Project Matters

This project is intentionally focused on the fundamentals that form the foundation of real-world analytics:

**Clean data → Validate data → Analyze patterns → Visualize results → Communicate business insights**

The goal is not simply to produce charts, but to demonstrate a repeatable analytical workflow from raw data to actionable observations.

---

## 📄 Project Status

**Status:** Completed Python EDA project

**Focus:** Data cleaning, exploratory analysis, visualization, and business insights

**Next stage:** Expand the project with stronger statistical analysis, interactive dashboards, and machine-learning use cases.
