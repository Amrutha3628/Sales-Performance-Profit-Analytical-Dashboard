Sales Performance & Profit Analytical Dashboard

📊 Project Overview

The Sales Performance & Profit Analytical Dashboard is an interactive Power BI project designed to analyze sales performance, profitability, customer orders, product performance, category contribution, regional performance, and business trends.

The project focuses on transforming raw sales data into meaningful business insights using Power Query, DAX, data visualization, interactive filtering, drill-down, drill-through, bookmarks, and navigation features.

⸻

🎯 Project Objectives

* Analyze overall sales and profit performance.
* Identify high-performing and low-performing products.
* Compare sales performance across regions.
* Analyze category-wise sales and profitability.
* Track sales, profit, and order trends over time.
* Calculate important business KPIs using DAX.
* Create an interactive and user-friendly Power BI dashboard.
* Provide business insights and recommendations based on the analysis.

⸻

🛠️ Tools & Technologies

* Microsoft Power BI
* Power Query
* DAX
* Data Visualization
* Data Cleaning & Transformation
* Interactive Dashboard Design

⸻

📁 Dataset

The project uses a sales dataset containing approximately 1,000 rows with the following fields:

* Order ID
* Order Date
* Customer Name
* Region
* Product
* Category
* Quantity
* Unit Price
* Sales
* Cost
* Profit
* Profit-Cost Difference

The original dataset contained missing values and duplicate records, which were handled during the data preparation stage.

⸻

🧹 Data Cleaning & Transformation

Data preparation was performed using Power Query.

The main cleaning activities included:

* Identified missing values in important columns.
* Removed duplicate records.
* Changed columns to appropriate data types.
* Converted Order Date to Date format.
* Handled missing Customer values.
* Handled missing Region values.
* Resolved missing Product values.
* Addressed missing Sales, Cost, and Profit values.
* Created cleaned Sales values using Quantity × Unit Price where required.
* Calculated missing Profit values using Sales − Cost.
* Created Profit-Cost Difference for profitability analysis.
* Standardized the final dataset for Power BI analysis.

⸻

🧮 DAX Calculations

Total Sales

Total Sales = SUM('SalesData_1000Rows_WithIssues_copy'[Sales])

Total Cost

Total Cost = SUM('SalesData_1000Rows_WithIssues_copy'[Cost])

Total Profit

TotalProfit = SUM('SalesData_1000Rows_WithIssues_copy'[Profit])

Total Quantity

Total Quantity = SUM('SalesData_1000Rows_WithIssues_copy'[Quantity])

Total Orders

Total Orders = COUNTROWS('SalesData_1000Rows_WithIssues_copy')

Average Order Value

Average Order Value =
DIVIDE([Total Sales], [Total Orders], 0)

Profit Margin

Profit Margin % =
DIVIDE([TotalProfit], [Total Sales], 0)

Profit-Cost Difference

A calculated column was created to compare profit against cost:

ProfitCostDifference =
'SalesData_1000Rows_WithIssues_copy'[Profit]
-
'SalesData_1000Rows_WithIssues_copy'[Cost]

East Region Orders

A calculated table was created to analyze orders from the East region.

⸻

📄 Dashboard Pages

1. Sales Performance Overview

This page provides a high-level summary of the overall business performance.

KPIs

* Total Sales
* Total Profit
* Profit Margin
* Total Orders
* Average Order Value

Visualizations

* Sales & Profit by Region
* Order Distribution by Region
* Monthly Sales Trend
* Sales vs Profit Trend
* Sales by Category
* Regional Sales Performance Map

Slicers

* Region
* Category
* Order Date

⸻

2. Regional Sales Analysis

This page focuses on regional sales and profitability performance.

Visualizations

* Profit Margin by Region
* Average Order Value by Region
* Category Sales by Region
* Sales Heatmap by Region & Category

Analysis

The page helps identify differences in sales contribution, profitability, order value, and category performance across regions.

⸻

3. Product & Category Analysis

This page provides detailed product and category-level analysis.

Visualizations

* Top 5 Trending Products
* Product Sales Performance
* Product Profit Performance
* Category Profit Analysis
* Sales vs Profit by Product

Top 5 Analysis

The Top 5 products were identified using the Total Orders measure.

Drill Down

The Category Profit Analysis visual uses:

Category → Product

This allows users to move from category-level performance to individual product-level performance.

Scatter Analysis

The Product Sales vs Profit analysis uses:

* X-axis → Total Sales
* Y-axis → Total Profit
* Legend → Product
* Tooltips → Sales, Profit, Orders, Quantity, Profit Margin

A trend line was also used to understand the relationship between sales and profit.

⸻

4. Sales & Profit Trend Analysis

This page focuses on time-based performance.

Visualizations

* Profit Trend Over Time
* Monthly Orders Trend
* Monthly Profit Margin Trend
* Year-wise Sales Performance
* Year-wise Profit Performance

Drill Down

The Order Date hierarchy supports:

Year → Quarter

This allows users to explore performance at a more detailed time level.

⸻

5. Insights & Recommendations

The final page summarizes the main business findings and recommendations from the dashboard.

Key Insights

* Regional sales contribution varies across the business.
* Product performance differs in terms of sales and order volume.
* Profitability varies across products and categories.
* Sales and profit trends change over time.
* Order volume helps identify stronger demand areas.

Recommendations

* Focus on products with strong sales and order performance.
* Review pricing and cost structures for lower-profit products.
* Monitor regional performance regularly.
* Track profit margin along with sales rather than focusing only on revenue.
* Use sales, profit, and order trends to support business decisions.

⸻

🔎 Interactive Features

The dashboard includes several Power BI interactive features.

Slicers

Used for:

* Region
* Category
* Order Date

Drill Down

Category → Product

Implemented in the Category Profit Analysis visual.

Drill Through

A dedicated Product Details page was created.

Users can right-click a product and select:

Drill through → Product Details

The Product Details table contains:

* Product
* Category
* Region
* Total Sales
* Total Profit
* Total Orders
* Total Quantity
* Total Cost

A Back button is available to return to the source page.

Page Navigation

Page navigation was added across the main dashboard pages.

Reset / Clear All

A Reset button with a bookmark was created on the main Overview page to return the report to its default filter state.

Tooltips

Additional measures were added to tooltips to provide more information without overcrowding the visuals.

⸻

🎨 Dashboard Design

The dashboard uses a dark professional theme with orange and green accents.

Main Colors

* Dark Background: #0B0B0B
* Orange Accent: #FF8C00
* Profit Green: #22C55E
* White Text: #FFFFFF
* Secondary Text: #CBD5E1

The dashboard maintains consistent spacing, alignment, typography, colors, and visual hierarchy across the pages.

⸻

📌 Key Learning Outcomes

Through this project, I gained practical experience in:

* Power Query data cleaning
* Handling missing values
* Removing duplicate records
* Data transformation
* DAX calculated columns
* DAX measures
* Calculated tables
* KPI creation
* Sales and profit analysis
* Regional analysis
* Product and category analysis
* Time-series analysis
* Interactive dashboard development
* Drill-down
* Drill-through
* Bookmarks
* Page navigation
* Slicers
* Tooltips
* Business insights and recommendations

⸻

📂 Repository Contents

PowerBI/
    Sales_Performance_Profit_Analytical_Dashboard.pbix
Dataset/
    SalesData_1000Rows_WithIssues_copy.xlsx
Documentation/
    Sales_Performance_Profit_Analytical_Dashboard_Documentation.pdf
Screenshots/
    Dashboard screenshots

⸻

🚀 Project Outcome

This project demonstrates how raw sales data can be transformed into an interactive business intelligence solution using Microsoft Power BI.

The final dashboard enables users to explore sales, profit, orders, products, categories, regions, and trends through interactive visualizations and analytical features.

⸻

👩‍💻 Author

Amrutha Asokan

Data Analyst Aspirant | Power BI | SQL | Python | Excel

⸻
