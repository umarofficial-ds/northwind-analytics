# Northwind Analytics: SQL Queries & Power BI Dashboard

A data analysis project on the classic **Northwind** database. It pairs 25 analytical SQL queries (PostgreSQL) with an interactive Power BI dashboard.

## Project Structure

```
.
├── Dashboard/
│   ├── NortWindDashboard.pbix   # Power BI source file
│   └── NortWindDashboard.pdf    # Static PDF export of the dashboard
├── dashboards/
│   ├── Ecommerce.jpeg           # Dashboard preview
│   ├── Food_Powerbi.jpeg        # Dashboard preview
│   └── Python.jpeg              # Dashboard preview
└── Sql_Query_Tasks/
    └── northwind.sql            # Northwind schema, data, and 25 query tasks
```

## SQL Tasks

`Sql_Query_Tasks/northwind.sql` creates the Northwind tables and data, followed by 25 queries in five groups:

| Group | Topics |
|---|---|
| Sales & Revenue | Monthly revenue trends, top 10 products, sales by country/year, average order value, year-over-year growth |
| Customer & Geography | Top customers by spend, inactive customers, customers per country, churn rate, order frequency |
| Product Performance | 3-month declining sales, margins per category, cross-sold products, percentile ranking, products never ordered |
| Employees & Territories | Sales per employee, revenue contribution %, territory growth, delivery delay, outperformers |
| Advanced / Analytical | Order ranking per customer, latest order, cumulative revenue, seasonality, order status funnel |

SQL concepts used: joins, aggregations, CTEs, subqueries, window functions, date functions.

## Power BI Dashboard

`Dashboard/NortWindDashboard.pbix` is the interactive report. Open it in Power BI Desktop, or view `NortWindDashboard.pdf` for a quick look.

## How to Use

1. Create a PostgreSQL database:
   ```bash
   createdb northwind
   ```
2. Load the script:
   ```bash
   psql -d northwind -f Sql_Query_Tasks/northwind.sql
   ```
3. Run the queries from the Tasks section at the bottom of the file.

## Tools

- PostgreSQL
- Microsoft Power BI Desktop

## Author

**Haider Khan**
