# Retail-Sales-Dashboard
An interactive Retail Sales Analysis Dashboard built with Microsoft Power BI and DAX to analyze sales performance, profitability, product categories, and regional trends through KPI cards and interactive visualizations.

![image alt](https://github.com/khadijahamidani/Retail-Sales-Dashboard/blob/4691f7897e72405efe8db491e2537c9d4f78d8f5/retail%20sales%20dashboard.JPG)

Retail Sales Analysis Dashboard | Power BI
Project Overview

This project focuses on analyzing retail sales data using Microsoft Power BI to gain insights into sales performance, profitability, product category performance, and regional sales distribution.

The dashboard transforms raw retail sales data into meaningful business insights through interactive visualizations and DAX measures. It helps users monitor key performance indicators (KPIs), identify sales trends, compare product categories, and evaluate profitability.

Objectives
Analyze overall retail sales and profit performance.
Monitor key business metrics through KPI cards.
Understand sales distribution across different regions.
Compare sales performance across product categories.
Track monthly sales trends and identify changes over time.
Analyze profit contribution by product category.
Support data-driven business decisions through visual analytics.
Tools and Technologies
Microsoft Power BI Desktop — Dashboard development and data visualization.
DAX (Data Analysis Expressions) — Creation of measures and KPI calculations.
Power Query — Data preparation and transformation, if applicable.
GitHub — Project documentation and version control.
Dataset Description

The dataset contains retail sales transaction information, including the following fields:

Column	Description
Order Date	Date of the retail transaction
Order ID	Unique identifier for an order
Product Category	Category to which a product belongs
Product Name	Name of the product sold
Discount	Discount applied to the transaction
Quantity	Number of units sold
Region	Geographic sales region
Retail Sales	Sales amount generated
Retail Profit	Profit earned from the transaction
Profit Margin	Profitability measure, if provided in the source data

Note: The dashboard's profit margin KPI is calculated using a DAX measure. Confirm whether the source dataset also contains a separate profit margin column.

Key Performance Indicators (KPIs)

The dashboard includes four key metrics:

Total Sales: Measures the total sales revenue generated.
Total Profit: Measures the total profit generated from retail transactions.
Total Quantity: Measures the total number of units sold.
Profit Margin: Evaluates profitability relative to sales, based on the defined DAX calculation.
Dashboard Visualizations
1. Sales by Region

A pie chart showing how total sales are distributed across different regions. It helps compare each region's contribution to overall sales.

2. Sales by Product Category

A clustered bar chart comparing total sales across product categories to identify categories generating higher revenue.

3. Monthly Sales Trend

A line chart displaying sales performance over time. It helps identify monthly increases, decreases, and potential seasonal patterns.

4. Profit by Product Category

A chart comparing total profit across product categories. It helps distinguish categories that generate higher profit from those that generate lower profit.

5. Monthly Sales and Profit Trend

If included in the final report, this combo chart uses columns for total sales and a line for total profit to compare their monthly movements.

DAX Measures

The following are representative examples of the measures used in the project. Adjust the table and column names to match the actual Power BI model.

Total Sales
Total Sales =
SUM('Retail Sales'[Retail Sales])

Total Profit
Total Profit =
SUM('Retail Sales'[Retail Profit])

Total Quantity
Total Quantity =
SUM('Retail Sales'[Quantity])

Profit Margin
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)


Format the profit margin measure as a percentage. These examples assume that retail profit and retail sales are additive transaction-level amounts.

Business Value

The dashboard can help stakeholders:

Monitor sales and profitability at a glance.
Compare regional sales performance.
Identify high-revenue product categories.
Understand monthly sales fluctuations.
Compare profitability across product categories.
Investigate areas that may require further business analysis.

The dashboard supports exploratory analysis; conclusions about causes of changes in sales or profit require additional investigation.

Project Structure

A suggested repository structure is:

retail-sales-analysis-powerbi/
├── README.md
├── dashboard/
│   └── retail-sales-dashboard.pbix
├── data/
│   └── retail-sales-data.csv
└── screenshots/
    └── dashboard-overview.png


Include only the files you actually upload. If the dataset is confidential or subject to licensing restrictions, do not publish it; provide a sample or data dictionary instead.

How to Use
Clone or download this repository.
Open the .pbix file using Microsoft Power BI Desktop.
If prompted, connect to the appropriate dataset or update the data source path.
Refresh the data if necessary.
Explore the dashboard and its available filters and visual interactions.
Key Learnings

Through this project, I practiced:

Building interactive dashboards in Power BI.
Creating DAX measures for business KPIs.
Comparing sales and profitability across dimensions.
Visualizing time-based sales trends.
Selecting visualizations to answer business questions.
Presenting retail data in a format that supports decision-making.
Future Improvements

Potential extensions include:

Sales growth and month-over-month analysis.
Top-performing products by profit.
Discount impact and profitability analysis.
More detailed time-based comparisons.

These are possible future enhancements and are not necessarily part of the current dashboard.

Author

Khadija Hamidani



This project was developed for learning and portfolio purposes to demonstrate skills in Power BI, DAX, data visualization, and retail sales analysis.
