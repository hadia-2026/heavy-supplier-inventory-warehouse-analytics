\# Week 01 Sprint Summary



\## Sprint Goal



Understand the structure, quality, relationships, and initial business meaning of the CodeTX supply-chain datasets.



\## Work Completed



\- Loaded all 12 project datasets

\- Reviewed dataset dimensions and column structures

\- Identified master and transaction tables

\- Profiled data types and missing values

\- Investigated duplicate identifiers

\- Checked exact duplicate rows

\- Validated major foreign-key relationships

\- Reviewed date ranges and converted date fields

\- Investigated missing purchase-order received dates

\- Validated the inventory product-branch composite key

\- Cleaned warehouse capacity into a numeric field

\- Performed numeric sanity checks

\- Validated current inventory against the stock ledger

\- Reviewed major categorical fields



\## Key Findings



\- No exact duplicate rows were found.

\- Duplicate `invoice\_id` and `payment\_id` values exist, but they belong to different transactions.

\- The 2,370 missing purchase-order received dates all correspond to cancelled purchase orders.

\- Major table relationships contain no unmatched foreign-key values.

\- Inventory contains one record for each of 30 products across 6 branches.

\- Current stock values match the latest stock-ledger balance for all 180 product-branch combinations.

\- Major categorical values are consistently formatted.



\## Deliverables



\- `01\_data\_understanding.ipynb`

\- Initial project README

\- Week 01 sprint documentation

\- Initial data-quality findings



\## Next Sprint



Week 02 will focus on data cleaning decisions, identifier handling, validation rules, and preparation of analysis-ready datasets.

