# Decision Log – Data Pipeline & Scraping

## Objective

This log explains the technical decisions made regarding which data extraction processes and transformation rules are automated within my ETL pipelines.

## Pipeline Components

1. Main Scraper (Data Extraction)
2. Data Cleaning (Transformation)
3. Error Notification (Monitoring)
4. Proxy Rotation
5. Image Downloading

## Decisions

### 1. Main Scraper (Data Extraction)

**Decision:** Automated
**Reason:** This is the core of the "Extract" phase. Automation is mandatory to ensure consistent data flow from the target source.

### 2. Data Cleaning (Transformation)

**Decision:** Automated
**Reason:** To ensure data integrity. Automated scripts remove duplicates and format dates/currencies before the "Load" phase.

### 3. Error Notification (Monitoring)

**Decision:** Automated
**Reason:** Critical for pipeline health. I need immediate alerts if the target website structure changes or the scraper fails.

### 4. Proxy Rotation

**Decision:** Pending / Conditional
**Reason:** Currently not required for low-volume scraping. Will be automated if rate-limiting becomes a bottleneck.

### 5. Image Downloading

**Decision:** Manual / Not Automated (Temporary)
**Reason:** High storage cost and not critical for the current data analysis phase. Focusing on textual data first.
