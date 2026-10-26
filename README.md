# FedEx Logistics Performance Analysis and Relational Database Design

## Project Overview

This project was completed as part of the **AlmaBetter Module 3 Capstone Project**. It focuses on designing and implementing a relational database using the SCMS Delivery History dataset and conducting SQL-based analysis of logistics and shipment delivery performance.

The project demonstrates how a structured relational database can support data integrity, efficient querying, and meaningful operational analysis.

## Objectives

- Examine and prepare the source dataset for relational database design.
- Identify entities, attributes, identifiers, and relationships.
- Design a normalized relational database schema.
- Implement the database using SQLite.
- Validate table structures and key relationships.
- Use SQL queries to analyze shipment delivery performance.
- Present key findings through visualizations.

## Tools and Technologies

- **Python:** Data preparation and validation.
- **Pandas:** Data inspection and analysis.
- **SQLite:** Relational database implementation.
- **SQL:** Data retrieval, joins, aggregations, and business analysis.
- **Google Colab / Jupyter Notebook:** Project development and documentation.
- **Matplotlib:** Data visualization.

## Database Design

The implemented database contains **12 related tables** covering entities and relationships associated with countries, manufacturing sites, products, projects, purchase orders, purchase requests, shipment modes, shipments, transaction lines, vendors, and related records.

The design uses relational database concepts such as primary keys, foreign keys, and relationship tables to represent connections between entities and reduce unnecessary data duplication.

## Data Validation

The project includes checks for database structure, record counts, key uniqueness, and foreign-key relationships. These checks help establish that the database is structurally consistent and suitable for SQL-based analysis.

## SQL-Based Business Analysis

The analysis examines:

- Overall shipment delivery status.
- Vendor-wise late-delivery performance.
- Shipment-mode performance.
- Country-wise delivery performance.
- Country and shipment-mode combinations.
- Largest contributors to late shipments.

The queries use techniques including Common Table Expressions (CTEs), joins, date calculations, conditional logic, aggregation, and grouped filtering.

## Key Findings

The shipment-level analysis covers **7,030 shipments**:

| Delivery status | Shipments | Percentage |
|---|---:|---:|
| On schedule | 4,450 | 63.30% |
| Early | 1,775 | 25.25% |
| Late | 805 | 11.45% |
| **Total** | **7,030** | **100%** |

The average delivery difference was **-4.77 days**, indicating earlier delivery on average under the date-calculation rule used in this project.

These findings are descriptive. They identify delivery patterns and areas for further investigation but do not establish the causes of delays.

## Project Notebook

The Jupyter Notebook contains the project workflow, including data importing and cleaning, database design, validation, SQL-based analysis, visualizations, and conclusions.

Open the notebook file listed in this repository to review the detailed implementation.

## Limitations

- Findings depend on the quality and completeness of the source dataset.
- Shipment-level delivery calculations use the project's stated scheduled-date rule.
- Differences in shipment volume should be considered when comparing late-shipment counts and percentages.
- The analysis identifies associations and patterns, not causal relationships.

## Acknowledgement

This project was completed as part of the AlmaBetter Module 3 Capstone Project on relational database design and logistics performance analysis.
