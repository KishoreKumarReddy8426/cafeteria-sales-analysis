# ☕ Cafeteria Sales Data Analysis

A Python data-analysis project that cleans and analyzes one year of cafeteria sales transactions to identify sales trends, product performance, purchasing patterns, and business insights using **Pandas, NumPy, Matplotlib, and Seaborn**.

> **Raw Data → Data Cleaning → Exploratory Data Analysis → Visualization → Insights → Recommendations**

## 📌 Project Overview

Raw transaction data can contain missing values, duplicate records, inconsistent entries, and invalid values. This project demonstrates a practical workflow for preparing cafeteria sales data and using Python to answer business questions.

The analysis focuses on:

- Monthly revenue trends
- Product performance
- Peak sales days
- Customer purchasing patterns
- Relationships between sales variables
- Data-quality issues
- Business recommendations

## 🎯 Business Objectives

- Analyze overall cafeteria sales performance
- Identify the highest and lowest revenue months
- Determine the best-selling products
- Identify peak sales days
- Study purchasing patterns
- Explore relationships between sales variables
- Generate data-driven business recommendations

## 📂 Dataset

| Attribute | Details |
|---|---|
| Dataset | Cafeteria Sales Data |
| File | `Cafeteria.csv` |
| Time Period | January 2023 – December 2023 |
| Total Transactions | 10,000 |
| Data Type | Transaction-level sales data |

## 🧹 Data Cleaning

The script performs the following preparation steps:

- Reports missing values and dataset information
- Removes rows missing critical transaction fields
- Removes rows containing `UNKNOWN` or `ERROR`
- Converts transaction dates to datetime
- Converts quantity and unit price to numeric values
- Removes rows that remain invalid after conversion
- Removes duplicate records
- Creates a calculated `Total Price` field

### Revenue Formula

```text
Total Price = Quantity × Price Per Unit
```

## 🔍 Exploratory Data Analysis

The project includes:

### Descriptive Statistics

- Mean
- Median
- Standard deviation
- Minimum and maximum values
- Distribution summary

### Correlation Analysis

The script calculates correlations between:

- Quantity
- Price Per Unit
- Total Price

**Important interpretation:** `Total Price` is calculated as `Quantity × Price Per Unit`, so its strong correlation with those variables is partly mathematical by construction. It should not be treated as evidence of an independent causal relationship.

### Sales Analysis

The script analyzes:

- Monthly revenue
- Top-selling products by quantity
- Revenue by day of week
- Peak sales days

## 📊 Visualizations

The Python script generates the following visualizations when executed:

1. **Correlation Heatmap** — relationship between Quantity, Price Per Unit, and Total Price
2. **Monthly Sales Bar Chart** — monthly revenue comparison
3. **Top Selling Items Bar Chart** — top 10 products by quantity sold
4. **Peak Sales by Day** — revenue comparison across days of the week

The charts are generated directly by `cafeteria_analysis.py` and are not stored as separate image files in this repository.

## 💡 Key Insights

Based on the current analysis:

- Most customer purchases contain **2–4 items**.
- **March** has the highest reported monthly revenue (**₹85,420**).
- **August** has the lowest reported monthly revenue (**₹61,280**).
- **Coffee** is the top-selling product by quantity.
- **Friday** records the highest reported sales volume.
- The strong Quantity–Total Price relationship is expected because Total Price is calculated from Quantity and Price Per Unit.

> The numerical results above are based on the current dataset and analysis script. Re-running the script will reproduce the calculated tables and charts.

## 🚀 Business Recommendations

### 📦 Inventory Management

Maintain appropriate stock levels for consistently high-selling products, especially Coffee, to reduce potential stock shortages.

### 🎁 Product Bundling

Consider combining lower-performing products with popular items in promotional bundles.

### 📅 Seasonal Promotions

Use low-performing months as opportunities for targeted promotions and demand-generation campaigns.

### 👥 Staffing Optimization

Use peak-day sales patterns to help plan staffing levels.

### 📊 Data Quality

Introduce validation rules during data entry to reduce missing, invalid, and inconsistent records.

## 🛠 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Pandas | Data cleaning, transformation, and analysis |
| NumPy | Numerical computation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |

## 🎯 Skills Demonstrated

- Python programming
- Pandas data cleaning
- Data wrangling
- Exploratory Data Analysis (EDA)
- Descriptive statistics
- Correlation analysis
- Data visualization
- Business insight generation
- Data-driven recommendations

## 📁 Project Structure

```text
cafeteria-sales-analysis/
│
├── Cafeteria.csv
├── cafeteria_analysis.py
├── README.md
└── Requirements_Document.pdf
```

## ⚙️ Installation & Usage

### 1. Clone the repository

```bash
git clone https://github.com/KishoreKumarReddy8426/cafeteria-sales-analysis.git
```

### 2. Navigate to the project

```bash
cd cafeteria-sales-analysis
```

### 3. Install dependencies

The script requires:

```text
pandas
numpy
matplotlib
seaborn
```

Install them with:

```bash
pip install pandas numpy matplotlib seaborn
```

### 4. Run the analysis

```bash
python cafeteria_analysis.py
```

The script prints data-quality reports, summary statistics, correlation results, monthly sales, top-selling items, and peak sales-day analysis. It also displays the generated charts.

## 🔮 Future Improvements

- Add a dedicated `requirements.txt` file
- Save generated charts in an `images/` directory
- Build an interactive Streamlit dashboard
- Develop Power BI and Tableau versions
- Add sales forecasting using machine learning
- Add customer segmentation
- Add interactive Plotly visualizations
- Automate report generation
- Deploy the analysis as a web application

## 👨‍💻 Author

### Kishore Kumar Reddy

**Data Analyst | Python | SQL | Tableau | Power BI**

Passionate about transforming raw data into meaningful insights through analytics, visualization, and business intelligence.

**GitHub:** [KishoreKumarReddy8426](https://github.com/KishoreKumarReddy8426)

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub. Feedback and suggestions are welcome.
