\# Week 4 Sprint Log — Product Performance Analysis



\## Objective

Evaluate product-level sales, revenue contribution, profitability, movement, and demand behavior using delivered sales only.



\## Work Completed



\### Product Performance Summary

\- Aggregated delivered sales into one row per product.

\- Preserved all 30 unique products.

\- Validated that aggregated product revenue exactly matched delivered sales revenue.

\- Calculated:

&#x20; - Total units sold

&#x20; - Total revenue

&#x20; - Estimated total cost

&#x20; - Estimated gross profit

&#x20; - Gross margin percentage

&#x20; - Order count

&#x20; - Customer count

&#x20; - Average revenue per order

&#x20; - Average units per order



\### Revenue Analysis

\- Ranked products by delivered sales revenue.

\- Calculated revenue contribution percentage.

\- Identified the highest-revenue products.

\- Compared revenue performance with sales volume and profitability.



\### ABC / Pareto Analysis

\- Ranked products by revenue contribution.

\- Calculated cumulative revenue percentage.

\- Classified products into:

&#x20; - Class A: 9 products

&#x20; - Class B: 7 products

&#x20; - Class C: 14 products

\- Created a Pareto visualization to show revenue concentration.



\### Product Movement Analysis

\- Evaluated movement using both total units sold and order frequency.

\- Created a percentile-based movement score.

\- Classified products as:

&#x20; - Fast Moving: 8

&#x20; - Medium Moving: 14

&#x20; - Slow Moving: 8

\- Movement classes are relative because product sales volumes are tightly distributed.



\### ABC vs Movement

\- Compared revenue importance with movement behavior.

\- Found that high-revenue products are not always fast-moving.

\- Some lower-revenue products show relatively high movement.

\- Combined ABC and movement characteristics into strategic priority groups.



\### Profitability Analysis

\- Evaluated gross margin performance across products.

\- Gross margins ranged from approximately 17% to 46%.

\- Created relative profitability classes:

&#x20; - High Margin

&#x20; - Medium Margin

&#x20; - Low Margin

\- Compared revenue contribution with profit contribution.



\### Category Performance

\- Aggregated product performance by product category.

\- Compared category revenue, units sold, gross profit, margin, and revenue contribution.



\### Monthly Demand Analysis

\- Created monthly sales history for each product.

\- Calculated:

&#x20; - Average monthly units

&#x20; - Minimum monthly units

&#x20; - Maximum monthly units

&#x20; - Monthly demand standard deviation

&#x20; - Demand coefficient of variation

\- Classified products into stable, moderate, and variable demand groups.



\### Strategic Product View

Product performance was evaluated across multiple dimensions:



\- Revenue importance

\- Sales movement

\- Profitability

\- Demand stability

\- Strategic priority



This avoids relying on a single KPI when evaluating product importance.



\## Key Findings

\- All 30 products were represented in delivered sales.

\- Delivered sales revenue was 22,958,987,430.

\- Product-level aggregation matched delivered revenue exactly.

\- Nine Class A products generated approximately the first 80% of cumulative revenue.

\- Product movement was relatively balanced across the dataset.

\- Revenue importance and product movement were not always aligned.

\- Gross margin percentages varied materially across products.

\- Product demand showed different levels of month-to-month stability.



\## Outputs Created

\- product\_performance.csv

\- category\_performance.csv

\- monthly\_product\_sales.csv

\- strategic\_products.csv



\## Key Learning

Product performance should not be judged using revenue alone.



A stronger evaluation combines revenue contribution, product movement, profitability, and demand stability.



\## Status

Week 4 completed successfully.

