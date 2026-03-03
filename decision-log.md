# Decision Log – Data Engineering & Pipeline Evolution

## Objective

This log explains the technical pivot from Web Scraping to a dedicated **ELT (Extract, Load, Transform)** focus.

## Strategic Pivot: From Scraping to ELT

**Date:** January 2026

**Decision:** Deprioritizing Web Scraping in favor of structured ELT Pipelines.

**Reason:** Scraping often suffers from high maintenance due to UI changes. ELT focuses on data architecture, scalability, and leveraging modern data warehouses, which aligns better with long-term data engineering goals.

## Updated Pipeline Components (ELT Focus)

1. **Extraction (E):** Focus on API integrations and Database CDC (Change Data Capture) instead of DOM parsing.
2. **Loading (L):** Prioritizing "Load First" to Cloud Storage (S3/GCS) or Data Warehouses (BigQuery/Postgres).
3. **Transformation (T):** Moving logic to SQL-based transformations (dbt style) post-loading.
4. **Monitoring:** Automated alerts for schema changes and pipeline failures via GitHub Actions.
