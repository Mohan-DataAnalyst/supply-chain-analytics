# Supply Chain Analytics

**Status: in progress.** Excel stage complete.
## About
ExcelR group project (team of 6). The goal is a dashboard of supply chain KPIs from order and inventory data. This repository holds my own work.

## Dataset
Training dataset from ExcelR: 12,000 orders (2023 to 2024), 6,228 monthly inventory rows and lookup tables for customers, products, suppliers and warehouses. The data file is not included here.

## KPIs
| KPI | Definition | Value |
|---|---|---|
| Total orders | Count of orders | 12,000 |
| Total sales revenue | Ordered quantity x unit price | $193.99M |
| Fill rate | Total shipped / total ordered | 96.9% |
| On-time delivery | Orders with status On-Time / all orders | 66.0% |
| Stock in hand | Stock at the latest snapshot (31 Dec 2024) | 782,208 |

Filters: year, region, country, ship mode.

## Visuals
Orders by region, orders by ship mode, top 5 cities by quantity, average lead time vs ship mode, re-order ratio by warehouse region, forecast vs actual demand.

## What I found
- About one third of orders were late: 2,239 slightly delayed and 1,837 delayed, out of 12,000.
- Sea shipments averaged about 29 days from order to delivery, against about 7 for air.
- Monthly demand stayed near 28,500 units in 2023, but August 2024 peaked at 38,178.
- No product was below its reorder level in the latest snapshot.

## How I worked
1. Kept the original data untouched and cleaned in Power Query.
2. Checked every table for blanks, duplicates, invalid dates and broken links, and logged each result (`docs/`).
3. Calculated fill rate from quantities, not from the source column, which disagreed with the quantities in about 1,700 rows.
4. Joined customer, product and warehouse details onto orders and inventory.
5. Built the KPIs and charts as PivotTables with slicers.

## Limits
- The data has no stock-out or address-error fields.
- The forecast is the 2023 monthly average. A trend method was tested and was about 27% off, so the average (about 7.5% off) was used. Method to be confirmed with the mentor.
- Stock figures use one snapshot, so the Year, Region and Ship Mode filters do not apply to them.

## My contribution
[Write what you did yourself, in your own words. Only what's true.]

## Files
- `images/`: dashboard screenshots
- `docs/`: cleaning log and KPI definitions

## About me
I moved from structural steel detailing into supply chain analytics. [LinkedIn](https://www.linkedin.com/in/endala-mohan-3b8515270)
