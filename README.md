# NYC Taxi Data Pipeline

This project processes NYC Taxi trip data using Azure Databricks.

Raw taxi data is ingested into the Bronze layer using incremental processing.
The Silver layer cleans the data, fixes data types, and removes duplicate trips.

In the Gold layer, dimension tables are created using SCD Type 1 and Type 2,
and a fact_trip table is built with one row per trip using UPSERT logic.

The final data is clean, reliable, and ready for reporting and analysis
using SQL or Power BI.
