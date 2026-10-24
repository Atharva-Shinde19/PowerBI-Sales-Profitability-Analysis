# 📊 Sales & Profitability Analysis Dashboard | Power BI

## 📌 Project Overview

This project uses Microsoft Power BI to analyze retail sales and profitability across different regions, product categories, and products.

The interactive dashboard helps users explore sales trends, compare regional performance, identify loss-making products, and investigate the relationship between discounts and profitability.

## 🎯 Business Objectives

- Analyze overall sales and profit performance.
- Compare sales across different regions.
- Identify the most and least profitable product categories.
- Investigate products generating negative profits.
- Explore the relationship between discounts and profitability.
- Present business insights through interactive visualizations.

## 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- CSV Dataset

## 📂 Dataset

The project uses a practice retail sales dataset containing 40 records and 11 columns.

Key fields include:

- Order ID
- Order Date
- Region
- State
- Category
- Sub-Category
- Product Name
- Quantity
- Sales
- Discount
- Profit

**Note:** This is a small practice dataset created for learning and demonstration purposes. It does not represent actual company data.

## 📈 Dashboard Pages

### 1. Executive Overview

Provides a high-level summary of business performance.

Key components:
- Total Sales
- Total Profit
- Total Orders
- Profit Margin
- Monthly Sales Trend
- Sales by Region
- Profit by Category
- Interactive date, region, and category filters

### 2. Product & Profit Analysis

Provides a more detailed view of product performance.

Key components:
- Profit by Product
- Profit by Sub-Category
- Product Performance Table
- Discount Analysis
- Interactive region and category filters

## 🧮 DAX Measures

The project includes the following measures:

**Total Sales**
```dax
Total Sales = SUM('SalesData'[Sales])
```

**Total Profit**
```dax
Total Profit = SUM('SalesData'[Profit])
```

**Total Orders**
```dax
Total Orders = DISTINCTCOUNT('SalesData'[Order ID])
```

**Total Quantity**
```dax
Total Quantity = SUM('SalesData'[Quantity])
```

**Profit Margin**
```dax
Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
```

**Average Discount**
```dax
Average Discount = AVERAGE('SalesData'[Discount])
```

## 💡 Key Learning Outcomes

- Data preparation and transformation using Power Query.
- Creating DAX measures for business KPIs.
- Designing interactive Power BI reports.
- Analyzing regional and product-level performance.
- Identifying negative-profit records.
- Translating data analysis into business recommendations.

## 🚀 How to Use

1. Download or clone this repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. If Power BI requests the dataset location, reconnect it to the CSV file in the `dataset` folder.
4. Refresh the data if required.
5. Explore the dashboard using the available slicers and visualizations.

## 📸 Dashboard Previews

### Executive Overview

Add the screenshot here.

### Product & Profit Analysis
![Executive Overview]
(ScreenShots/ExecutiveOverview.png)


## 📌 Conclusion

This project demonstrates the use of Power BI, Power Query, and DAX to transform retail sales data into interactive dashboards and business insights.

It serves as a practical learning project in data analytics and business intelligence.
