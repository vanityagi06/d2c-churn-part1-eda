# Data Quality Report
## Missing Values
### customers.csv
* loyalty_tier: 1386 missing values
* skin_type: 401 missing values

### orders.csv
* rating: 80 missing values

## Duplicate-like Records
The orders dataset contains intentionally created duplicate-like records identified by the "_DUP" suffix in the order_id column.

## Outlier Analysis
Potential outliers were identified in:
* gross_amount
* delivery_days
* resolution_hours

These records should be reviewed before modelling but may represent valid business events.

## Join Integrity
All datasets successfully joined using customer_id.
No orphan customer records were detected.
The customer table can therefore be used as the primary entity table.
