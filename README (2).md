# SuperStore Sales & Forecasting Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![DAX](https://img.shields.io/badge/DAX-Analytics-blue)
![Power Query](https://img.shields.io/badge/Power%20Query-Data%20Transformation-green)
![Forecasting](https://img.shields.io/badge/Analytics-Sales%20Forecasting-orange)
![Retail Analytics](https://img.shields.io/badge/Domain-Retail%20Analytics-purple)

## 📊 Project Overview

The **SuperStore Sales & Forecasting Dashboard** is an interactive Power BI project that analyzes sales, profit, orders, returns, shipping performance, customer segments, product categories, regions, and state-level performance.

The project also includes a dedicated **15-day sales forecasting page**, extending the dashboard beyond historical reporting into forward-looking analysis.

The objective is to transform transactional sales data into an interactive business intelligence solution that helps stakeholders understand performance, identify trends, and support sales planning.

---

## 🎯 Business Objectives

- Monitor overall sales and profitability.
- Track order volume and returns.
- Analyze sales performance by region and state.
- Compare sales across customer segments.
- Analyze product category and subcategory performance.
- Understand payment-mode distribution.
- Evaluate shipping-mode performance.
- Compare monthly sales and profit across years.
- Identify high-performing states and categories.
- Generate a short-term sales forecast.
- Provide an interactive executive-level view of business performance.

---

## 🛠️ Tools & Technologies

- **Power BI** — Dashboard development and interactive visualization
- **Power Query** — Data cleaning and transformation
- **DAX** — KPI calculations and analytical measures
- **Power BI Forecasting** — Short-term sales forecasting
- **Data Visualization** — KPI cards, donut charts, line charts, bar charts, maps, and tables
- **Business Intelligence** — Sales and profitability analysis

---

## 📌 Key KPIs

The main dashboard displays the following KPIs:

| KPI | Dashboard Value |
|---|---:|
| Total Sales | **1.6M** |
| Total Orders | **22K** |
| Total Profit | **175K** |
| Average Ship Days | **4** |
| Total Returns | **287** |

> KPI values are based on the dashboard view shown in this project.

---

## 📈 Dashboard Analysis

### 1. Sales by Payment Mode

The dashboard analyzes sales distribution across different payment methods:

- Cash on Delivery (COD)
- Online
- Cards

This provides insight into customer payment preferences.

### 2. Sales by Region

Sales are compared across the four major regions:

- Central
- East
- South
- West

The dashboard also provides regional navigation for interactive analysis.

### 3. Sales by Segment

Customer sales are analyzed across:

- Consumer
- Corporate
- Home Office

This helps identify the customer segment contributing the most revenue.

### 4. Monthly Sales — Year over Year

The dashboard compares monthly sales across **2019 and 2020** to identify:

- Seasonal patterns
- Growth or decline
- High-performing months
- Changes in sales momentum

### 5. Monthly Profit — Year over Year

Monthly profit is compared across years to understand profitability trends and identify periods of stronger or weaker performance.

### 6. Sales by Category

Sales are analyzed across major product categories, including:

- Office Supplies
- Technology
- Furniture

### 7. Sales by Subcategory

The dashboard highlights top-performing subcategories such as:

- Phones
- Chairs
- Binders

This helps identify product groups contributing significantly to sales.

### 8. Sales by Ship Mode

Sales are compared across shipping methods:

- Standard Class
- Second Class
- First Class
- Same Day

This provides a view of how sales are distributed across delivery options.

### 9. Profit and Sales by State

The geographic analysis provides a state-level view of business performance and helps identify high-performing markets.

---

# 🔮 Sales Forecasting

A dedicated dashboard page provides a **15-day sales forecast**.

The forecast page contains:

- Historical sales trend
- Short-term forecast period
- Recent sales behavior
- State-level sales comparison
- A detailed view of the most recent sales period

The forecast is intended to support short-term sales planning and trend analysis.

### Forecasting Methodology

**Important:** The exact forecasting methodology should be documented according to the method used in the Power BI file.

If the forecast was created using Power BI's built-in Analytics-pane forecasting functionality, describe it as:

> **Power BI built-in time-series forecasting**

If a custom forecasting model was used, document the specific model and validation approach here.

Do not describe the dashboard as an ML forecasting project unless a machine-learning/statistical forecasting model was actually developed and evaluated.

---

## 🔍 Key Business Observations

Based on the dashboard:

- Total sales are approximately **1.6M**.
- Total profit is approximately **175K**.
- The dashboard contains approximately **22K orders**.
- Average shipping time is approximately **4 days**.
- The dashboard records **287 returns**.
- **West** contributes the largest displayed share of regional sales.
- **Consumer** is the largest customer segment in the displayed analysis.
- **Phones** are among the highest-performing displayed subcategories.
- **Standard Class** is the largest shipping-mode category by sales.
- The sales forecast page provides a short-term forward-looking view of sales performance.

> These observations are descriptive and should be validated against the underlying dataset and Power BI model before being used for operational decisions.

---

## 🖥️ Dashboard Preview

### Sales Dashboard

![SuperStore Sales Dashboard](Screenshots/SuperStore_Sales_Dashboard.png)

### Sales Forecast Dashboard

![SuperStore Sales Forecast](Screenshots/SuperStore_Sales_Forecast.png)

---

## ⚙️ Data Preparation

The dataset was prepared using **Power Query** before dashboard development.

The preparation process included:

- Reviewing the source data
- Cleaning and transforming columns
- Validating data types
- Preparing categorical fields
- Creating analysis-ready data
- Building relationships/measures required for reporting

---

## 🧮 DAX & Measures

The dashboard uses DAX measures to calculate important business metrics such as:

- Total Sales
- Total Orders
- Total Profit
- Average Ship Days
- Total Returns
- Sales by Region
- Sales by Category
- Sales by Subcategory
- Profit by Month

Example:

```DAX
Total Sales =
SUM('SuperStore Data'[Sales])
```

Example profit measure:

```DAX
Total Profit =
SUM('SuperStore Data'[Profit])
```

> Update the table and column names in these examples if your Power BI data model uses different names.

---

## 🎛️ Dashboard Features

- Interactive region selection
- KPI cards
- Cross-filtering
- Sales and profit trend analysis
- Geographic state-level analysis
- Category and subcategory analysis
- Shipping-mode analysis
- Customer-segment analysis
- Year-over-year comparison
- Dedicated sales forecasting page

---

## 💡 Business Value

The dashboard can help business stakeholders:

- Monitor revenue and profitability.
- Identify high-performing regions and states.
- Understand customer segment contribution.
- Identify high-performing products and categories.
- Analyze shipping preferences.
- Track returns.
- Compare year-over-year sales and profit.
- Use short-term forecasts to support sales planning.

---

## 🚀 Future Improvements

Potential enhancements include:

- Add **Profit Margin %**.
- Add **Year-over-Year Growth %**.
- Add **Sales per Order**.
- Add **Return Rate %**.
- Add **Profit by State** ranking.
- Add **Top 10 / Bottom 10 Products**.
- Add forecast accuracy metrics such as **MAE, RMSE, or MAPE** when an appropriate validation framework is available.
- Add drill-through pages for product and state analysis.
- Add dedicated tooltip pages.
- Add an executive **Key Insights** panel.
- Improve accessibility and visual consistency.

---

## 📂 Project Structure

```text
SuperStore-Sales-Forecasting-PowerBI/
│
├── README.md
├── SuperStore_Sales_Dashboard.pbix
│
├── Dataset/
│   └── SuperStore.csv
│
└── Screenshots/
    ├── SuperStore_Sales_Dashboard.png
    └── SuperStore_Sales_Forecast.png
```

---

## 👤 Author

**Pratik More**

Data Analyst | Power BI | SQL | Python | Data Analytics

---

⭐ If you find this project useful, consider giving the repository a star.
