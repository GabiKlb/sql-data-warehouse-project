# SQL Data Warehouse Project

## Overview

This project simulates the end-to-end design and implementation of a modern Data Warehouse using SQL.

The objective is to model, transform, and structure raw business data into an analytical layer optimized for reporting and decision-making.

## Architecture

This project follows a Medallion Architecture pattern to progressively refine data quality and structure.

### Bronze Layer (Raw Data)
- Source CSV files ingested without transformation
- Preserves original structure for traceability

### Silver Layer (Staging)
- Data cleansing and type casting
- Null handling and validation
- Deduplication logic
- Standardization of formats

### Gold Layer (Data Warehouse)
- Dimensional modeling (Star Schema)
- Fact and dimension tables
- Surrogate key implementation
- Optimized for analytical queries

The star schema was chosen to:
- Simplify analytical queries
- Improve aggregation performance
- Enhance maintainability
