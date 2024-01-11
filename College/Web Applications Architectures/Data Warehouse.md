## Definition

A **data warehouse** is a centralized repository that stores large volumes of structured data from multiple sources. Its primary purpose is to facilitate reporting and analysis.

## Characteristics

- **Subject-Oriented**: Focuses on modelling and analysis of data for decision-making.
- **Integrated**: Consolidates data from various sources into a coherent whole.
- **Non-Volatile**: Once entered into the warehouse, data is not changed.
- **Time-Variant**: Data is stored in a way to allow comparisons over time.

## Architecture

1. **Data Sources**: Can include databases, flat files, online transaction processing (OLTP) systems.
2. **Data Extraction**: Data is extracted from the sources.
3. **Data Cleaning and Transformation**: Ensures data quality and converts it into a suitable format.
4. **Data Loading**: Data is loaded into the warehouse periodically.
5. **Storage**: Stores data in a structured format, often using dimensional or relational models.
6. **Data Access Tools**: Used for querying, reporting, and analysis (e.g., [[SQL]], Business Intelligence tools).

## Types

- **Enterprise Data Warehouses (EDW)**: Offers a centralized version of truth for the whole organization.
- **Operational Data Stores (ODS)**: More focused on operational level reporting.
- **Data Marts**: Subsets of data warehouses tailored for specific lines of business or departments.

## Benefits

- **Improved Decision Making**: Centralized data aids in making informed decisions.
- **Enhanced Data Quality and Consistency**: Standardizes data across the organization.
- **Historical Intelligence**: Allows analysis of large volumes of historical data for trends and patterns.

## Challenges

- **Data Integration**: Combining data from different sources can be complex.
- **Data Management**: Requires effective strategies for data storage, archiving, and retrieval.
- **Security and Privacy**: Ensuring data is securely stored and accessed.
- **Cost**: Can be expensive to implement and maintain.

## Use Cases

- **Business Intelligence**: For reporting and decision-making.
- **Data Mining**: Discovering patterns and relationships in large datasets.
- **Customer Relationship Management (CRM)**: To understand and predict customer behaviours.