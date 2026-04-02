# Ford Vehicle Sales & Valuation – ETL & Data Warehouse

ETL pipeline and data warehouse for analyzing Ford vehicle sales and valuations.

## Tech Stack
- **SSIS** (SQL Server Integration Services) – ETL pipeline
- **SQL Server** – Data warehouse
- **Power BI** – Dashboards and reporting

## Architecture
Constellation schema with shared dimensions and two fact tables:

- `FactSales` – vehicle sales transactions
- `FactValuation` – vehicle valuation data

### Dimensions
`DimVehicle` · `DimCustomer` · `DimSeller` · `DimLocation` · `DimTime`

## ETL Pipeline
Data is loaded from flat CSV files, transformed (cleaning, surrogate key generation, dimension lookups) and loaded into the data warehouse via SSIS packages.
