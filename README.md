
# Online Retail Sales Analytics Dashboard 🛒

## Project Overview
Built a fully interactive single page Power BI dashboard 
analyzing 500,000+ retail transactions to provide 
business insights for CEO and CMO decision making.

This project was completed as part of the
**Tata Group Data Visualisation Job Simulation on Forage.**

## Problem Statement
The CEO and CMO of an online retail store wanted answers 
to 4 key business questions:
1. How did monthly revenue trend in 2011?
2. Which top 10 countries generate highest revenue?
3. Who are the top 10 highest value customers?
4. Which regions have highest global demand?

## Tools Used
- Power BI Desktop
- DAX (Data Analysis Expressions)
- MS Excel / CSV

## Dataset
- Raw records: 541,909 transactions
- Clean records: 397,924 rows
- Period: 2010 - 2011
- Columns: InvoiceNo, StockCode, Description,
  Quantity, InvoiceDate, UnitPrice, 
  CustomerID, Country

## Data Cleaning Steps
1. Removed Quantity < 1 (returned orders)
2. Removed UnitPrice < 0 (data entry errors)
3. Removed blank CustomerID rows
4. Created Revenue = Quantity x UnitPrice
5. Created Month and Year columns

## Dashboard Features
✅ 6 KPI Cards — Total Revenue, Orders, 
   Countries, Customers, Avg Order Value, 
   Total Quantity Sold
✅ Monthly Revenue Trend Line Chart (2011)
✅ Top 5 Countries by Revenue (Excl. UK)
✅ Top 10 Customers by Revenue
✅ Global Demand World Map (Excl. UK)
✅ Average Order Value by Country
✅ Monthly Sales Volume Trend
✅ Interactive Slicers — Year, Month, 
   Country, Customer

## Key Business Insights
📈 November 2011 was peak revenue month — $1.15M
   indicating strong holiday season demand

🌍 Netherlands is top international market 
   with $280K revenue outside UK

👤 Customer 14646 is highest value customer
   contributing $280K in revenue

🗺️ Europe shows strongest global demand —
   ideal region for business expansion


## DAX Measures Created
- Revenue = Quantity x UnitPrice
- Revenue 2011 = CALCULATE(SUM Revenue, Year = 2011)
- Revenue Ex UK = CALCULATE(SUM Revenue, 
  Country != United Kingdom)
- Quantity Ex UK = CALCULATE(SUM Quantity,
  Country != United Kingdom)
- Total Revenue = SUM of Revenue

## Project Files
| File | Description |
|---|---|
| Retail_Dashboard.pbix | Power BI Dashboard |
| Clean_Retail_Data.csv | Cleaned Dataset |
| dashboard_screenshot.png | Dashboard Preview |

## Skills Demonstrated
- Data Cleaning and Preparation
- DAX Formula Writing
- Power BI Dashboard Development
- Business Intelligence
- Data Visualisation
- Stakeholder Reporting

