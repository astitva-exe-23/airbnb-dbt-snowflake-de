# End-to-End Data Engineering Pipeline with AWS S3, Snowflake & DBT

## Overview

This project demonstrates an end-to-end modern Data Engineering workflow using AWS S3, Snowflake, and DBT.

The pipeline follows the Medallion Architecture (Bronze → Silver → Gold) and implements industry-standard practices such as incremental loading, upserts, metadata-driven transformations, dimensional modeling, SCD Type 2 tracking, and data quality testing.

## Architecture

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/2760656c-39b2-42de-9c5b-2af21481a5a3" />

## Tech Stack

- AWS S3
- Snowflake
- DBT (Data Build Tool)
- SQL
- Jinja
- Git & GitHub

---

## Key Concepts Implemented

### Snowflake

- Database & Schema Creation
- External Stages
- File Formats
- IAM Integration
- Data Loading using `COPY INTO`

### DBT Fundamentals

- Models
- Sources
- Materializations
- Profiles Configuration
- Project Configuration

### Jinja & Macros

- Dynamic SQL generation
- Reusable transformation logic
- Custom schema generation
- Metadata-driven SQL patterns

### Incremental Processing

- Incremental Models
- Watermark-based loading
- Upsert logic
- Unique Key based merges

### Data Modeling

- One Big Table (OBT)
- Star Schema Design
- Fact Tables
- Dimension Tables

### Historical Tracking

- DBT Snapshots
- Slowly Changing Dimension Type 2 (SCD Type 2)

### Data Quality

- Generic Tests
- Singular Tests
- Source Data Validation
- Quality Gates before downstream propagation

---

## Project Structure

```text
.
├── models
│   ├── bronze
│   ├── silver
│   ├── gold
│   └── sources.yml
│
├── macros
│   ├── custom_schema.sql
│   └── reusable_macros.sql
│
├── snapshots
│
├── tests
│
├── dbt_project.yml
│
└── profiles.yml
```

---

## Features

- End-to-end ELT pipeline
- AWS S3 → Snowflake ingestion
- Incremental loading strategy
- Upsert implementation
- Metadata-driven transformations
- Reusable Jinja macros
- Star schema modeling
- Historical tracking with snapshots
- Data quality testing framework

---

## Lessons Learned

During this project I gained hands-on experience with:

- Snowflake ingestion architecture
- DBT project structure
- Jinja templating and macros
- Incremental processing patterns
- Metadata-driven pipeline design
- Dimensional data modeling
- SCD Type 2 implementation
- Data quality validation practices

---

## Future Improvements

- Automated orchestration using Airflow
- CI/CD integration with GitHub Actions
- Environment-specific deployments
- Advanced testing framework
- Monitoring and alerting
- Data lineage visualization

---

## Author

Astitva Singh

Data Engineering | Snowflake | DBT | AWS****
