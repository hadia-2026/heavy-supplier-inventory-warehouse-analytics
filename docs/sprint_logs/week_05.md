\# Week 5 Sprint Log — Inventory Analytics



\## Objective

Evaluate inventory value, stock movement, turnover-related behavior, stock health, and inventory risk using historical inventory and stock-ledger data.



\## Work Completed



\### Inventory Value Analysis

\- Calculated product-level inventory value.

\- Analysed inventory value by product, branch, and category.

\- Calculated each product's contribution to total inventory value.



\### Integration with Product Performance

\- Connected Week 5 inventory analysis with Week 4 product-performance classifications.

\- Combined inventory value with:

&#x20; - ABC class

&#x20; - Product movement class

&#x20; - Profitability class

&#x20; - Demand stability

&#x20; - Product priority

\- Created an exploratory inventory-risk framework.



\### Inventory Risk Classification

Products were classified into:

\- Strategic Inventory

\- High Holding Risk

\- Monitor Slow Movement

\- Normal Review



The classification combines product revenue importance and relative product movement.



\### Inventory Coverage Investigation

\- Calculated an exploratory months-of-stock indicator using current stock and average monthly demand.

\- Values ranged from approximately 1,071 to 1,197 months.

\- These values were operationally unrealistic and consistent with the inventory-scale anomaly identified in earlier weeks.

\- The metric was therefore excluded from final operational KPI use.



\### Historical Stock Movement Analysis

Historical stock-ledger transactions were used to calculate:

\- Total stock IN

\- Total stock OUT

\- Adjustment quantities

\- Stock-in event frequency

\- Stock-out event frequency

\- Out-to-in ratio

\- Net stock flow



The out-to-in ratio was relatively similar across products, averaging approximately 5.5%.



\### Relative Inventory Turnover

Because a standard accounting inventory turnover ratio could not be calculated reliably from the available inventory snapshot, a relative turnover indicator was developed using:

\- Historical stock-out quantity

\- Stock-out event frequency

\- Week 4 product movement score



Products were classified as:

\- High Turnover: 8

\- Medium Turnover: 14

\- Low Turnover: 8



\### Inventory Action Framework

Product revenue importance and relative turnover were combined into an inventory action framework:



\- Protect Availability: 2 products

\- Maintain Supply: 6 products

\- Standard Control: 14 products

\- Monitor Inventory: 6 products

\- Reduce / Review Holding: 2 products



\### Product-Level Stock Activity

Product-level stock activity was evaluated using the stock ledger.



All products showed recent stock activity, with days since last movement ranging from 0 to 9 days.



This indicated that no product could confidently be classified as dead stock at the overall product level.



\### Product-Branch Stock Health

Stock activity was then evaluated at the product-branch level.



Across 180 product-branch combinations:

\- Minimum days since last movement: 0

\- Median: approximately 10 days

\- Maximum: 28 days



A relative stock-health framework classified combinations as:



\- Normal: 97

\- Monitor Activity: 35

\- Healthy Movement: 33

\- Potential Stagnation: 15



Potential Stagnation represents combinations with both lower recent activity and low product turnover.



\### Stagnation Concentration

Potential stagnation was analysed by product and branch.



Kolkata East Depot showed the highest number of flagged product-branch combinations.



Transmission Assembly TA-800 showed the strongest product-level stagnation concentration, appearing in multiple branches.



These findings provide a direct link between inventory health and the Week 6 warehouse-performance analysis.



\## Data Limitation



A systematic scale inconsistency exists between current inventory balances and configured inventory thresholds.



Because of this:

\- Current-stock-to-max-stock ratios are not used as final operational KPIs.

\- Months-of-stock values are not used for optimization recommendations.

\- Inventory-value figures associated with flagged records are used mainly for relative comparison.

\- Historical stock movements and relative classifications are prioritized for inventory-health analysis.



\## Outputs Created

\- product\_inventory\_value.csv

\- inventory\_turnover\_strategy.csv

\- product\_branch\_stock\_health.csv

\- stagnation\_by\_branch.csv

\- stagnation\_by\_product.csv



\## Key Learning

Inventory optimization should not rely on a single stock-level metric.



A stronger approach combines:

\- Product importance

\- Historical movement

\- Relative turnover

\- Recent activity

\- Warehouse-level stock behavior



The analysis also demonstrated the importance of rejecting operationally unrealistic KPIs when data limitations make them unreliable.



\## Status

Week 5 completed successfully.

