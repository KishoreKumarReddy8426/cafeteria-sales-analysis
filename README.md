# ☕ Cafeteria Sales Data Analysis

<p align="center">

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C9BE8)

</p>

A comprehensive **Python Data Analysis** project that analyzes one year of cafeteria sales transactions to uncover sales trends, customer purchasing behavior, product performance, and business insights using **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn**.

The project follows a complete analytics workflow:

> **Raw Data → Data Cleaning → Exploratory Data Analysis → Data Visualization → Business Insights → Recommendations**

---

# 📌 Project Overview

Every cafeteria generates thousands of sales transactions, but raw transaction data often contains missing values, duplicate records, inconsistent entries, and invalid values that reduce its usefulness for business decision-making.

This project demonstrates how Python can be used to clean, analyze, and visualize cafeteria sales data to answer important business questions and generate actionable recommendations.

The analysis focuses on identifying:

- Monthly revenue trends
- Product performance
- Peak sales periods
- Customer purchasing behavior
- Correlation between sales variables
- Revenue-driving factors
- Opportunities to improve inventory management and sales

---

# 🎯 Business Objectives

The primary objectives of this analysis are:

- Analyze overall cafeteria sales performance
- Identify the highest and lowest revenue months
- Determine the best-selling products
- Identify peak sales days
- Study customer purchasing patterns
- Understand relationships between sales variables
- Generate business recommendations based on data

---

# 📂 Dataset

| Attribute | Details |
|-----------|---------|
| Dataset | Cafeteria Sales Data |
| File | `Cafeteria.csv` |
| Time Period | January 2023 – December 2023 |
| Total Transactions | **10,000** |
| Data Type | Transaction-Level Sales Data |

---

# 📊 Results Summary

| Metric | Result |
|---------|---------|
| 📄 Total Transactions | **10,000** |
| 💰 Revenue Calculation | Quantity × Price Per Unit |
| 📈 Highest Revenue Month | **March (₹85,420)** |
| 📉 Lowest Revenue Month | **August (₹61,280)** |
| ☕ Top Selling Product | **Coffee** |
| 📅 Peak Sales Day | **Friday** |
| 🔗 Strongest Correlation | Quantity Sold ↔ Total Price (**0.91**) |
| 🛒 Average Purchase Size | **2–4 Items** |

---

# 🧹 Data Cleaning

The dataset was cleaned before analysis to improve data quality and ensure accurate results.

### Data Cleaning Activities

- Removed missing values
- Removed duplicate records
- Handled invalid values (`UNKNOWN`, `ERROR`)
- Converted date columns into datetime format
- Corrected data types
- Validated numerical columns
- Created a **Total Price** column

### Revenue Formula

```text
Total Price = Quantity Sold × Price Per Unit
```

---

# 🔍 Exploratory Data Analysis (EDA)

The following analyses were performed:

### 📈 Descriptive Statistics

- Mean
- Median
- Standard Deviation
- Minimum
- Maximum
- Distribution Analysis

### 🔗 Correlation Analysis

Correlation analysis was performed to understand relationships between:

- Quantity Sold
- Price Per Unit
- Total Price

### 📊 Sales Trend Analysis

The project analyzes:

- Monthly Revenue
- Product Performance
- Peak Sales Days
- Seasonal Trends
- Customer Purchasing Behavior

---

# 📊 Visualizations

## 🔗 Correlation Heatmap

The heatmap illustrates relationships between numerical variables.

<img src="https://github.com/user-attachments/assets/3770d4f9-5b86-4810-aafa-89d8cd14e7bb" width="800">

---

## 📈 Monthly Revenue

Monthly revenue analysis identifies seasonal demand and revenue fluctuations.

<img src="https://github.com/user-attachments/assets/9b45620e-0157-4118-ac66-42c1fd49ecd4" width="850">

---

## 🏆 Top Selling Products

Visualization of the highest-selling cafeteria products.

<img src="https://github.com/user-attachments/assets/42b3a5b3-fe98-44c0-b1c5-60cf6f4e8774" width="700">

---

## 📅 Peak Sales Days

Analysis of customer traffic across different days of the week.

<img src="https://github.com/user-attachments/assets/2f137eba-81db-40d2-a867-3459cc1e788b" width="550">

---

# 💡 Key Insights

The analysis revealed several important business findings:

- Most customer purchases contain **2–4 items**.
- Quantity Sold has a **strong positive correlation (0.91)** with Total Revenue.
- **March** generated the highest monthly revenue (**₹85,420**).
- **August** generated the lowest monthly revenue (**₹61,280**).
- **Coffee** is the best-selling product.
- **Friday** consistently records the highest sales volume.
- Revenue is primarily driven by sales volume rather than pricing.
- Data cleaning significantly improved the reliability of the analysis.

---

# 🚀 Business Recommendations

Based on the findings, the following recommendations are proposed.

## 📦 Inventory Management

Maintain higher stock levels for consistently high-selling products, especially Coffee, to reduce stock shortages.

## 🎁 Product Bundling

Introduce combo offers that combine low-performing products with popular items.

## 📅 Seasonal Promotions

Launch promotional campaigns during low-performing months to improve revenue.

## 👥 Staffing Optimization

Increase staffing levels during Fridays and other peak sales periods.

## 📊 Improve Data Quality

Implement validation rules during data entry to reduce missing values and invalid records.

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Cleaning & Analysis |
| NumPy | Numerical Computation |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |

---

# 🎯 Skills Demonstrated

This project demonstrates proficiency in:

- Python Programming
- Data Cleaning
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Correlation Analysis
- Business Intelligence
- Data Visualization
- Business Reporting
- Insight Generation
- Data-Driven Decision Making

---

# 📁 Project Structure

```text
cafeteria-sales-analysis/
│
├── data/
│   └── Cafeteria.csv
│
├── images/
│   ├── heatmap.png
│   ├── monthly_sales.png
│   ├── top_items.png
│   └── peak_sales_day.png
│
├── cafeteria_analysis.py
├── README.md
├── requirements.txt
└── Requirements_Document.pdf
```

---

# ⚙ Installation

### Clone the Repository

```bash
git clone https://github.com/KishoreKumarReddy8426/cafeteria-sales-analysis.git
```

### Navigate to the Project

```bash
cd cafeteria-sales-analysis
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Project

```bash
python cafeteria_analysis.py
```

---

# 📦 Requirements

```text
pandas
numpy
matplotlib
seaborn
```

---

# 🔮 Future Improvements

Future enhancements include:

- Build an interactive Streamlit dashboard
- Develop a Power BI dashboard
- Create Tableau dashboards
- Implement Sales Forecasting using Machine Learning
- Add Customer Segmentation
- Integrate Plotly interactive charts
- Deploy as a web application
- Add automated report generation

---

# 👨‍💻 Author

## Kishore Kumar Reddy

**Data Analyst | Python | SQL | Tableau | Power BI**

Passionate about transforming raw data into meaningful insights through analytics, visualization, and business intelligence.

**GitHub**

https://github.com/KishoreKumarReddy8426

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

Your feedback and suggestions are always appreciated!
