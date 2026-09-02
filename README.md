# ☕ Cafeteria Sales Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Data%20Processing-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C9BE8)

A **Python-based data analysis project** that explores one year of cafeteria sales transactions to identify sales trends, product performance, data quality issues, and actionable business insights using **Pandas, NumPy, Matplotlib, and Seaborn**.

---

## 📌 Project Overview

Cafeterias generate thousands of transactions throughout the year. However, raw transaction data often contains missing values, duplicate records, inconsistent entries, and invalid values.

This project performs **data cleaning and exploratory data analysis (EDA)** on cafeteria sales data from **2023** to understand:

* How sales change over time
* Which products generate the most sales
* Which days have higher sales
* How quantity and price influence revenue
* Whether there are seasonal sales patterns
* What business decisions can be supported by the data

The project follows a complete data analysis workflow:

**Raw Data → Data Cleaning → EDA → Visualization → Insights → Business Recommendations**

---

## 🎯 Business Objectives

The analysis aims to answer the following business questions:

1. What are the overall sales and revenue trends?
2. Which products are the best sellers?
3. Which months generate the highest revenue?
4. Which days of the week have the highest sales?
5. How does quantity sold impact revenue?
6. How does price per unit impact revenue?
7. Are there seasonal patterns in sales?
8. What actions can improve inventory and sales performance?

---

## 📂 Dataset

| Attribute    | Details                             |
| ------------ | ----------------------------------- |
| Dataset      | Cafeteria Sales Data                |
| File         | `Cafeteria.csv`                     |
| Period       | January 1, 2023 – December 31, 2023 |
| Transactions | 10,000                              |
| Data Type    | Transaction-level sales data        |

---

## 🧹 Data Cleaning

The dataset was cleaned and prepared before performing the analysis.

### Data Cleaning Steps

* Identified missing values
* Removed duplicate records
* Handled invalid values such as `UNKNOWN` and `ERROR`
* Converted columns to appropriate data types
* Converted date columns into datetime format
* Validated numerical columns
* Created a **Total Price** column

### Revenue Calculation

Revenue was calculated using:

```text
Total Price = Quantity Sold × Price Per Unit
```

---

## 🔍 Exploratory Data Analysis

The following analysis was performed:

### 📊 Descriptive Statistics

* Mean
* Median
* Minimum
* Maximum
* Standard deviation
* Distribution of numerical variables

### 🔗 Correlation Analysis

Correlation analysis was performed to understand relationships between numerical variables such as:

* Quantity Sold
* Price Per Unit
* Total Price

### 📈 Sales Trend Analysis

The project analyzes:

* Monthly revenue
* Product sales
* Daily sales
* Peak sales periods
* Seasonal trends

---

## 📊 Visualizations

### 🔗 Correlation Heatmap

The correlation heatmap helps identify relationships between numerical variables.

<img src="https://github.com/user-attachments/assets/3770d4f9-5b86-4810-aafa-89d8cd14e7bb" width="788">

---

### 📈 Monthly Sales

Monthly revenue was analyzed to identify high-performing and low-performing periods.

<img src="https://github.com/user-attachments/assets/9b45620e-0157-4118-ac66-42c1fd49ecd4" width="838">

---

### 🏆 Top Selling Items

The analysis identifies products with the highest sales volume.

<img src="https://github.com/user-attachments/assets/42b3a5b3-fe98-44c0-b1c5-60cf6f4e8774" width="703">

---

### 📅 Peak Sales Days

Sales were analyzed by day to identify periods of higher customer demand.

<img src="https://github.com/user-attachments/assets/2f137eba-81db-40d2-a867-3459cc1e788b" width="500">

---

## 💡 Key Insights

The analysis produced the following business observations:

* Most purchases contain approximately **2–4 items**.
* Revenue is strongly influenced by **Quantity Sold** and **Price Per Unit**.
* Certain months generate significantly higher revenue, indicating possible seasonal demand.
* A relatively small number of products contribute significantly to overall sales.
* Some days of the week consistently demonstrate stronger sales performance.
* Data quality issues such as `UNKNOWN`, `ERROR`, missing values, and duplicates can affect analysis accuracy.

---

## 🚀 Business Recommendations

Based on the analysis, the following actions could help improve cafeteria operations:

### 📦 Inventory Optimization

Maintain higher inventory levels for consistently high-selling products to reduce the possibility of stock-outs.

### 🎁 Combo Offers

Introduce combo deals or promotional offers for lower-performing products to increase their sales.

### 📅 Seasonal Promotions

Use historical sales patterns to plan promotions during low-sales months.

### 👥 Staffing Optimization

Increase staffing during peak sales periods to improve service efficiency and reduce customer waiting time.

### 🧹 Data Quality Improvements

Implement validation rules at the point of data entry to reduce invalid values such as `UNKNOWN` and `ERROR`.

---

## 🛠️ Technologies Used

| Technology     | Purpose                          |
| -------------- | -------------------------------- |
| **Python**     | Data analysis and processing     |
| **Pandas**     | Data cleaning and transformation |
| **NumPy**      | Numerical operations             |
| **Matplotlib** | Data visualization               |
| **Seaborn**    | Statistical visualization        |

---

## 📁 Project Structure

```text
cafeteria-sales-analysis/
│
├── Cafeteria.csv
├── cafeteria_analysis.py
├── README.md
├── Requirements_Document.pdf
│
└── images/
    ├── monthly_sales.png
    ├── top_items.png
    ├── heatmap.png
    └── peak_sales_day.png
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/KishoreKumarReddy8426/cafeteria-sales-analysis.git
```

### 2. Navigate to the Project

```bash
cd cafeteria-sales-analysis
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Analysis

```bash
python cafeteria_analysis.py
```

---

## 📦 Requirements

The project requires the following Python libraries:

```text
pandas
numpy
matplotlib
seaborn
```

---

## 🔮 Future Improvements

The project can be extended further by:

* 📊 Building an interactive **Streamlit dashboard**
* 📈 Developing a **Power BI dashboard**
* 🔮 Implementing sales forecasting using **Machine Learning**
* 👥 Adding customer segmentation
* 📊 Creating interactive visualizations using **Plotly**
* ☁️ Deploying the project to a cloud platform
* 🤖 Adding an AI-powered sales insights feature

---

## 🎓 Skills Demonstrated

This project demonstrates practical experience in:

* Python Programming
* Data Cleaning
* Data Transformation
* Exploratory Data Analysis
* Statistical Analysis
* Data Visualization
* Correlation Analysis
* Business Intelligence
* Business Insight Generation
* Data-driven Decision Making

---

## 👨‍💻 Author

### Kishore Kumar Reddy

**Data Analyst | Tableau Developer | Power BI Developer**

Interested in **Data Analytics, Business Intelligence, Python, SQL, Tableau, Power BI, and Data Science**.

🔗 **GitHub:**
https://github.com/KishoreKumarReddy8426

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a ⭐ on GitHub.

Your feedback and suggestions are always welcome!
