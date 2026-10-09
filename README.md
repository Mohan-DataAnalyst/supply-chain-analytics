# Supply Chain Analytics

**Status: in progress.** Items are ticked only when they are done.

## About
This is an ExcelR group project (team of 6). The goal is to build an Excel dashboard that tracks supply chain KPIs from order and inventory data. This repository holds my own work on the project.

## Dataset
- A supply chain dataset provided by ExcelR for training
- 7 sheets: orders (12,000 rows), inventory (6,228 monthly rows), and lookup tables for customers, products, suppliers and warehouses
- The data file is not included here

## KPIs the project needs
- Total orders
- Total sales revenue
- Fill rate
- Stock in hand
- On-time delivery

Filters: region or country, year, ship mode.

## How I work
1. Keep the original file untouched.
2. Check each table before using it.
3. Clean in Power Query, so every step is saved and can be read.
4. Write down every check and its result, even when nothing is found.
5. Write each KPI definition in one sentence before building it.

## Progress
- [x] Set up folders and made a copy of the data
- [x] Turned each sheet into a named table
- [x] Set the data types in Power Query
- [x] Checked and cleaned the Product table
- [ ] Supplier, Warehouse and Customer tables
- [ ] Inventory table
- [ ] Orders table
- [ ] Join the lookup tables to orders
- [ ] KPI definitions
- [ ] PivotTables and dashboard

## What is in this repository
- `docs/`: cleaning log and screenshots of Power Query steps

## About me
I moved from structural steel detailing into supply chain analytics. [LinkedIn](https://www.linkedin.com/in/endala-mohan-3b8515270)
