# Inventory Optimization Project Report
## Understanding Stock Changes and Smarter Planning

## What Is This All About?
- We noticed some stock issues; things going missing, running out, or being manually adjusted.
So, we decided to dive into our inventory logs and product data to figure out what’s really happening.

## The Big Question
Why are some products always out of stock or being changed manually?

## This project explores:
- Which products are affected
- How often inventory is being changed
- And how we can do better with planning

## Data Source
 ### Two datasets powered this analysis:
- Inventory Logs: each record is a stock change (like received, sold, adjusted)
- Product table: gives context (name, category, brand, price, etc.)

## Data Cleaning and Preparation
Before jumping in:
- Messy characters (like ₦ or $, and missing units of measure) were removed.
- The change_type column was standardized.
- Grouped change_type into categories (sales, manual, received).

## Vizualization
![](https://github.com/ESTHER-AKINTUNDE/Inventory_Analysis/blob/main/Dashboard.png)

## Key Insights:
- Products with IDs: PROD0021, PROD0014, PROD0030 etc. were adjusted manually a lot, maybe a sign of error or backdoor processes.
- A few Products such as PROD0004, PROD0011 and PROD0007 were frequently out of stock  leading to potential missed sales.
- Other products with IDs: PROD0001, PROD0020, PROD0009 etc. were barely touched, maybe overstocked or not selling.

## Suggestions/Recommendation
- We need better logging for timestamps
- Set reorder alerts for fast-selling products
- Train staff on reducing manual stock corrections (very important)
- Identify slow-moving stock and take action.
- Catch stock issues early
- Support smarter procurement
- Improve overall stock control
