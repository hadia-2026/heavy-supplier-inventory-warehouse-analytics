# Week 3 Sprint Log — Data Integration & Feature Engineering

## Objective
Integrate the cleaned datasets into reusable analytical tables and engineer business features for later analysis.

## Work Completed

### Sales Integration
- Integrated sales order lines with order headers, products, customers, and branches.
- Preserved line-level grain with 130,402 rows.
- Created time-based features including year, month, month name, and quarter.
- Created estimated cost, gross profit, and gross margin features.
- Used delivered orders for realized customer sales analysis.

### Procurement Integration
- Integrated purchase order lines with purchase order headers, products, suppliers, and branches.
- Preserved purchase-order-line grain.
- Created delivery delay, actual lead time, purchase-period, and delivery-performance features.
- Distinguished purchase-order-level delivery KPIs from line-level procurement data to prevent double counting.

### Inventory Integration
- Integrated inventory with product and branch information.
- Preserved 180 unique product-branch combinations.
- Created inventory value, excess stock, excess inventory value, stock status, and stock-to-max ratio features.
- Identified a systematic scale anomaly between current inventory balances and configured maximum-stock thresholds.
- Treated excess-stock indicators as exploratory rather than final KPIs.

### Warehouse Integration
- Created one analytical row per branch.
- Aggregated sales, inventory, workforce, operating cost, and stock movement information.
- Created sales-per-employee, operating-cost ratio, and stock-out-to-stock-in ratio metrics.
- Created transparent branch rankings without introducing an unjustified composite score.

### Supplier Integration
- Created one analytical row per supplier.
- Calculated purchase-order volume, procurement value, delivery delay, on-time rate, late rate, cancellation rate, and received-order delivery rates.
- Separated overall on-time rate from received-order on-time rate.

### Customer Integration
- Created one analytical row per customer.
- Calculated total sales, delivered order count, total units purchased, product variety, average order value, recency, tenure, and average units per order.
- All 500 customers had at least one delivered order.

## Key Findings
- 72.47% of purchase orders were delivered on time.
- 13.61% were late.
- 9.88% were cancelled.
- 4.05% were delivered early.
- Supplier received-order on-time rates were approximately 80%–81%.
- Chennai South Hub had the highest branch sales value.
- Kolkata East Depot showed the highest sales value per employee.
- Average customer sales value was approximately 45.92 million.
- Average delivered orders per customer were approximately 36.
- Average order value was approximately 1.27 million.
- Inventory threshold comparisons revealed a systematic scale anomaly requiring cautious interpretation.

## Analytical Datasets Created
- sales_analysis.csv
- procurement_analysis.csv
- inventory_analysis.csv
- warehouse_analysis.csv
- supplier_analysis.csv
- customer_analysis.csv

## Key Learning
A major focus of Week 3 was understanding dataset grain and preventing double counting. Header-level metrics were not directly aggregated from line-level integrated tables when repeated values could distort results.

## Status
Week 3 completed successfully.