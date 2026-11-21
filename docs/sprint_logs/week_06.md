\# Week 6 Sprint Log — Warehouse Analytics



\## Objective

Evaluate warehouse performance using stock movement, capacity, workforce, sales productivity, operating cost, stagnation, and product–warehouse alignment.



\## Work Completed



\### Warehouse Throughput

Historical stock-ledger transactions were aggregated by branch to calculate:



\- Total stock IN

\- Total stock OUT

\- Adjustment quantity

\- Total movement volume

\- Total movement events

\- Outbound share of total movement



Chennai South Hub recorded the highest raw total movement volume and the highest number of stock movement events.



\### Capacity-Adjusted Throughput

Raw movement volume was normalized using warehouse capacity and workforce.



Calculated indicators included:



\- Movement volume per square foot

\- Movement events per employee

\- Stock-out units per employee



This distinction allowed warehouses to be compared on relative operational intensity rather than raw size alone.



\### Sales and Workforce Efficiency

Warehouse performance was further evaluated using:



\- Sales per square foot

\- Units sold per employee

\- Operating-cost ratio



These indicators provide complementary views of commercial and operational efficiency.



\### Inventory Stagnation Integration

Week 5 product-branch stagnation findings were integrated into warehouse analysis.



A branch-level stagnation rate was calculated to show the percentage of products at each warehouse associated with potential stagnation.



\### Warehouse Bottleneck Screening

Four relative indicators were used:



\- Low sales density

\- Low throughput density

\- High operating-cost ratio

\- High stagnation rate



Results:



\- Delhi Central: High Bottleneck Risk

\- Hyderabad Logistics: Moderate Bottleneck Risk

\- Pune Distribution: Watch

\- Chennai South Hub: Watch

\- Kolkata East Depot: Watch

\- Ahmedabad West Hub: Watch



Delhi Central triggered all four bottleneck indicators.



\### Bottleneck Reasons

Specific bottleneck reasons were recorded for each warehouse to make the classification interpretable.



Examples include:



\- Low Sales Density

\- Low Throughput Density

\- High Operating Cost

\- High Stagnation



\### Warehouse Benchmarking

Warehouses were ranked separately using:



\- Sales density

\- Throughput density

\- Workforce productivity

\- Cost efficiency

\- Stock health



Separate rankings were used instead of an arbitrary weighted composite score.



\### Product–Warehouse Alignment

Week 4 product importance and Week 5 stock health were combined to evaluate product placement.



Across 180 product-branch combinations:



\- Standard Alignment: 162

\- Strong Alignment: 8

\- Strategic Misalignment: 6

\- Low-Priority Stagnation: 4



Strategic Misalignment identifies Class A products that show potential stagnation at a specific warehouse.



\### Strategic Misalignment by Warehouse

Kolkata East Depot showed the highest concentration of strategic misalignment, with two Class A products showing potential stagnation.



Ahmedabad West Hub, Delhi Central, Hyderabad Logistics, and Pune Distribution each showed one case.



Chennai South Hub showed no strategic misalignment cases.



\## Key Findings



\- Chennai South Hub had the highest raw stock movement volume.

\- Raw throughput and capacity-adjusted throughput produced different interpretations.

\- Delhi Central showed the strongest relative bottleneck profile.

\- Hyderabad Logistics showed moderate bottleneck risk.

\- Kolkata East Depot had the highest concentration of strategic product–warehouse misalignment.

\- Warehouse performance should be evaluated using multiple normalized indicators rather than raw activity alone.



\## Outputs Created



\- warehouse\_throughput.csv

\- warehouse\_benchmark.csv

\- product\_warehouse\_alignment.csv

\- misalignment\_by\_branch.csv

\- final\_warehouse\_view.csv



\## Key Learning

Warehouse performance cannot be evaluated reliably using raw movement or sales alone.



Capacity, workforce, operating cost, inventory health, and product importance must be considered together to identify meaningful bottlenecks and alignment issues.



\## Status

Week 6 completed successfully.

