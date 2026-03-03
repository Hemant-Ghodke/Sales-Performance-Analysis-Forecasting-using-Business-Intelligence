# 📊 Sales Performance Analysis & Forecasting using Business Intelligence

## 🚀 Project Overview

This project presents an end-to-end **Business Intelligence (BI) and Predictive Analytics solution** for retail sales performance analysis.

The system transforms raw transactional data into meaningful insights using:

- Data Preprocessing  
- KPI-driven performance monitoring  
- Interactive Power BI Dashboard  
- Time-Series Forecasting using ARIMA  

The objective is to demonstrate how Business Intelligence and Data Science techniques can be integrated to build a **data-driven decision support system**.

## 🎯 Problem Statement

Retail businesses generate massive volumes of transactional sales data across regions, product categories, customer segments, and time periods. However, many organizations struggle to convert raw data into actionable insights.

Traditional reporting systems are:

- Static  
- Spreadsheet-based  
- Time-consuming  
- Non-interactive  

Additionally, forecasting is often based on historical trends and managerial intuition rather than statistical models. This can lead to:

- Poor demand estimation  
- Inefficient inventory management  
- Suboptimal marketing strategies  
- Revenue loss  

This project addresses these challenges by building a centralized BI system integrated with predictive analytics.

## 🎯 Objectives

- Design a complete BI pipeline from raw data to dashboard
- Clean and preprocess transactional sales data
- Define and compute meaningful KPIs:
  - Total Sales
  - Total Profit
  - Profit Margin (%)
  - Total Orders
  - Average Order Value
- Build interactive Power BI visualizations
- Identify trends and seasonality
- Implement ARIMA-based sales forecasting
- Provide actionable business recommendations

## 📂 Dataset Description

### 📌 Source
- Superstore Sales Dataset  
- Sourced from Kaggle  
- Simulates real-world retail sales transactions  

### 📊 Dataset Size
- ~9,994 records  
- 21 attributes  

### 🏷 Attribute Categories

**Order Details**
- Order ID
- Order Date
- Ship Date
- Ship Mode

**Customer Information**
- Customer ID
- Customer Name
- Segment

**Geographical Data**
- Country
- City
- State
- Region

**Product Information**
- Category
- Sub-Category
- Product Name

**Financial Metrics**
- Sales
- Profit
- Quantity
- Discount

## 🧹 Data Preprocessing

### ✔ Handling Missing Values
- Numerical fields → Imputed using median
- Categorical fields → Filled with "Unknown"
- Invalid dates removed for time-series integrity

### ✔ Data Cleaning
- Standardized column names
- Converted date fields to datetime format
- Removed duplicate records
- Validated numerical values

### ✔ Outlier Detection
- Used Interquartile Range (IQR) method
- Removed non-representative extreme values
- Preserved natural seasonality for forecasting

### ✔ Feature Engineering
- Extracted Year, Month, Quarter
- Calculated Profit Margin (%)
- Aggregated monthly sales for ARIMA forecasting

## 📊 BI Dashboard (Power BI)

### 🔑 KPIs Displayed
- 💰 Total Sales: ₹460.63K  
- 📈 Total Profit: ₹71.23K  
- 📦 Total Orders: 4K  
- 📊 Profit Margin: 15.46%  
- 🧾 Average Order Value: ₹62.31  

### 📈 Visualizations

1. **Monthly Sales Trend with Forecast**
   - Historical sales
   - ARIMA-based 3-month forecast
   - Confidence interval band

2. **Sales by Category**
   - Office Supplies
   - Furniture
   - Technology

3. **Sales by Region**
   - West
   - East
   - Central
   - South

4. **Top Products Table**
   - Ranked by sales performance

5. **Year-wise Sales Trend**
   - Growth analysis (2014–2017)

### 🎛 Interactive Filters
- Year
- Region
- Category
- Customer Segment

## 🔮 Predictive Model

**Model Used:** ARIMA (1,1,0)

### Forecasting Process
1. Aggregated transaction data into monthly totals
2. Converted data into time-series format
3. Applied ARIMA model
4. Generated 3-month forward forecast
5. Integrated predictions into Power BI dashboard

This enhances the system from descriptive analytics to predictive analytics.

## 📈 Key Insights

- Certain regions contribute significantly higher revenue.
- A small subset of products drives the majority of total sales.
- Clear seasonal sales patterns are observed.
- High revenue does not always imply high profitability.
- Forecast indicates continued growth trend.

## 💡 Business Recommendations

- Focus marketing efforts on high-performing regions and categories
- Use forecast insights for inventory planning
- Optimize discount strategies for low-margin products
- Diversify revenue sources beyond top-performing products
- Institutionalize KPI monitoring using BI dashboards

## 🏗 Project Structure
Sales_BI_Project/
│
├── superstore.csv # Raw dataset (Superstore sales data)
│
├── main.py # Python script for preprocessing & forecasting
├── notebook.ipynb # Jupyter notebook (analysis + visualization)
│
├── report.docx # Final project report
│
├── outputs/ # Generated BI-ready files & visual outputs
│ ├── kpis.csv # Computed KPIs
│ ├── monthly_sales.csv # Aggregated monthly sales
│ ├── sales_by_region.csv # Sales grouped by region
│ ├── sales_by_category.csv # Sales grouped by category
│ ├── top_products.csv # Top 10 products by sales
│ ├── monthly_sales_trend.png # Historical sales trend chart
│ ├── sales_forecast_next_3_months.csv # ARIMA forecast results
│ └── sales_forecast.png # Forecast visualization
│
└── dashboard/
└── sales_dashboard.pbix # Power BI dashboard file

### Structure Explanation
- **Dataset** → Contains raw transactional data.
- **Python Scripts / Notebook** → Perform data cleaning, feature engineering, KPI computation, and ARIMA forecasting.
- **Outputs Folder** → Stores processed datasets and visualizations used in the BI dashboard.
- **Dashboard Folder** → Contains the Power BI dashboard file.
- **Report** → Detailed documentation of methodology, insights, and recommendations.

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels (ARIMA)
- Power BI

## 📌 Business Impact

This project demonstrates how combining:

- Data Cleaning  
- KPI Analytics  
- Interactive Dashboards  
- Statistical Forecasting  

can significantly enhance:

- Strategic planning  
- Inventory optimization  
- Revenue forecasting  
- Data-driven decision-making  

## 👨‍💻 Author

**Hemant Ghodke**  
BSc IT | Business Intelligence & Data Analytics  
