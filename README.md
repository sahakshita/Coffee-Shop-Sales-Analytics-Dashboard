# ☕ Coffee Shop Sales Analysis: MySQL and Power BI

![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black)

## 📌 Overview

An end-to-end sales analysis of a three-store coffee shop, using **MySQL** to clean the data and answer business questions, and **Power BI** to build an interactive dashboard. The data covers 149,116 transactions from 1 January to 30 June 2023 (Astoria, Hell's Kitchen and Lower Manhattan).

This project was built following the Coffee Shop Sales project by Data Tutorials (YouTube).

## 📊 Dashboard Preview

![Coffee Shop Sales Dashboard](coffee_shop_dashboard.png)

*Dashboard view with March 2023 selected. The interactive version, including the hover tooltips, is in the `.pbix` file.*

## 🛠️ Tools and Skills Used

- 🐬 **MySQL:** data cleaning (`STR_TO_DATE`, `ALTER TABLE`, `UPDATE`), aggregation (`SUM`, `COUNT`, `AVG`, `ROUND`), date functions (`MONTH`, `DAY`, `DAYOFWEEK`, `HOUR`), `CASE` statements, subqueries, and window functions (`LAG() OVER`, `AVG() OVER`) for month-over-month growth
- 📈 **Power BI:** KPI cards with month-over-month change, calendar heat map, sales trend with average line, weekday vs weekend split, sales by store, category and product, and an hour-by-day heat map
- 🖱️ **Custom tooltips:** hovering over a day in the calendar, or a cell in the hour-by-day heat map, opens a tooltip page showing sales, orders and quantity with a sales growth comparison

## 💡 Key Insights

**📅 Overall (Jan-Jun 2023):** total sales of **$698.8K** from **149,116** transactions and **214,470** units sold. Monthly sales grew from $81,678 in January to $166,486 in June (+103.8%).

**🚀 May 2023 (compared with April):**

- Sales were **$156,728** (+31.77%), orders were **33,527** (+32.33%) and units sold were **48,233** (+32.26%).
- The average sale stayed at about $4.69 every month, so growth came from more customers and items, not higher prices.
- 🌅 Mornings drive sales: 8:00 to 10:59 am brings in **36.8%** of May sales, and 10 am is the busiest hour.
- Weekdays made 74.4% of sales and weekends 25.6%, but May had 23 weekdays and 8 weekend days. Per day, sales were almost equal ($5,071 vs $5,012).
- ☕ Coffee (38.5%) and Tea (28.4%) together make up **66.9%** of sales. The top 10 product types bring 79.2%.
- 🏪 The three stores are almost equal: Hell's Kitchen 33.6%, Astoria 33.5% and Lower Manhattan 33.0%.

The full write-up with recommendations is in `Coffee_Shop_Sales_Insights.pdf`.

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `coffee_shop_sales_dashboard.pbix` | Power BI report file (open with Power BI Desktop) |
| `coffee_shop_sales_dashboard.pdf` | PDF export of the dashboard |
| `coffee_shop_dashboard.png` | Dashboard image used in this README |
| `MY_SQL_Queries.pdf` | All MySQL queries with their outputs |
| `Coffee_Shop_Sales_Insights.pdf` | Insights report with findings and recommendations |
| `Coffee_Shop_Sales.xlsx` | Raw transaction data |
