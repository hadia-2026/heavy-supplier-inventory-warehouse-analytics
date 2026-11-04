# Week 02 Sprint Summary

## Sprint Goal

Clean, validate, and prepare the CodeTX supply-chain datasets for reliable downstream analysis.

## Work Completed

- Investigated duplicate invoice and payment identifiers
- Created unique analytical record IDs
- Added ambiguity quality flags
- Standardized date fields
- Converted warehouse capacity into a numeric analysis-ready field
- Validated product and inventory business rules
- Validated purchase-order and sales-order dates and financial values
- Validated invoice and payment logic
- Reconciled purchase-order headers with line items
- Reconciled sales-order headers with line items
- Validated invoices against sales orders
- Investigated payment-to-invoice ambiguity
- Preserved all valid records
- Created cleaned copies of all datasets
- Exported 12 processed CSV files

## Key Findings

- Duplicate invoice and payment IDs represent identifier-integrity issues, not exact duplicate rows.
- Payment behavior is consistent when invoice IDs are unique.
- Ambiguous invoice IDs should not be used for reliable invoice-to-payment reconciliation.
- All 180 inventory records are above configured maximum stock levels, indicating a potential overstocking issue rather than a cleaning error.
- Purchase-order and sales-order financial calculations are internally consistent.
- No valid transaction rows were removed during cleaning.

## Deliverables

- `notebooks/02_data_cleaning.ipynb`
- 12 cleaned CSV files in `data/processed/`
- Week 02 sprint documentation
- Identifier-quality flags and validation results

## Next Sprint

Week 03 will focus on data integration, feature engineering, analytical table creation, and preparation for product, inventory, warehouse, supplier, and customer analysis.