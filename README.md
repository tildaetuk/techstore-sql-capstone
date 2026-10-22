# TechStore Inc. Sales Analysis (SQL Capstone)

Customer and sales analysis using SQL for TechStore Inc., an e-commerce company that sells electronics, furniture and accessories.

## Project Overview

I worked as a data analyst for TechStore Inc. Management wanted to improve sales performance, understand customer behaviour and optimise inventory. I wrote 20 SQL queries to answer their questions and turned the results into insights and recommendations.

Built for the SQL Capstone Final Project, AWE Mentorship, Month 3.


## The Data

The project uses four tables:

| Table | Columns | What it tells us |
|-------|---------|------------------|
| Customers | 7 | Who buys |
| Products | 6 | What is sold |
| Orders | 6 | What happened |
| Sales_Reps | 4 | Who sells |


## Key Findings

- **Revenue:** $147,140 from 163 completed orders, about $903 per order, from 18 active customers. All amounts are in USD (assumed, as the dataset does not state a currency).
- **Order status:** 78% Completed, 20% Pending (42 orders), 2% Cancelled (4 orders).
- **Top customers:** The top 10 customers bring in 86% of sales. John Smith is first with $18,480. The USA is the top country ($28,380), then India ($22,220).
- **Inactive customers:** 9 customers have stopped buying.
- **Age and gender:** Ages 25 to 44 bring in 92% of sales. Male customers spend about 64% more in total than female customers, with the same number of customers (9 each).
- **Products:** Office Chair Deluxe sells the most units (56), but Laptop Pro 14 earns the most money ($40,300 from 31 units). 11 of the 25 products had no completed sales.
- **Monthly sales:** Electronics earns the most every month. Sales peaked in March ($26,030) and fell to $18,510 in July.
- **Sales reps:** Africa and Oceania earned $28,460 with no sales reps. North America is the top region with 3 reps. South America has 1 rep but no sales.
- **Inventory:** The Standing Desk has the highest demand-to-stock ratio (0.90), so it should be restocked first.

- ## Recommendations

1. **Restock** the Standing Desk, Office Chair Deluxe and Laptop Pro 14.
2. **Add sales reps** in Africa and Oceania, and review South America.
3. **Win customers back** with a campaign for the 9 inactive customers.
4. **Close Pending orders** by following up the 42 Pending orders.
5. **Review slow products** by promoting, discounting or dropping the 11 products with no sales.
6. **Investigate the dip** in sales after March and check the July data.

## SQL Skills Used

SELECT, JOIN, GROUP BY and aggregations, filtering, CTEs, window functions (LAG) and date functions.

## Files

- `techstore_queries.sql`: all 20 queries used in this project

## Author
Matilda Etuk

1. Only **Completed** orders count as sales. Pending and Cancelled orders are not finished sales.
2. The Orders table has no SalesRepID column, so sales reps are analysed by **region**.
