# Advanced SQL Assignment

This repository contains my solutions for an Advanced SQL assignment covering
Common Table Expressions (CTEs), Views, Stored Procedures, Triggers,
Data Modelling, Normalization, and SQL data analysis.

## Topics Covered

- Common Table Expressions (CTEs)
- Updatable and Read-Only Views
- Stored Procedures
- Database Triggers
- Data Modelling
- Database Normalization
- Revenue Calculation
- Aggregate Functions
- SQL Views
- Stored Procedures with Parameters
- AFTER DELETE Triggers

## Assignment Questions

### Q1
What is a Common Table Expression (CTE), and how does it improve SQL query readability?

### Q2
Why are some views updatable while others are read-only?

### Q3
What advantages do stored procedures offer compared to writing raw SQL queries repeatedly?

### Q4
What is the purpose of triggers in a database?

### Q5
Explain the need for data modelling and normalization.

### Q6
Calculate total revenue for each product using a CTE.

### Q7
Create the `vw_CategorySummary` view.

### Q8
Create an updatable product view and update a product price.

### Q9
Create a stored procedure to retrieve products by category.

### Q10
Create an AFTER DELETE trigger to archive deleted products.

## Database Schema

### Products

| Column | Data Type | Description |
|---|---|---|
| ProductID | INT | Primary Key |
| ProductName | VARCHAR(100) | Product name |
| Category | VARCHAR(50) | Product category |
| Price | DECIMAL(10,2) | Product price |

### Sales

| Column | Data Type | Description |
|---|---|---|
| SaleID | INT | Primary Key |
| ProductID | INT | Foreign Key |
| Quantity | INT | Quantity sold |
| SaleDate | DATE | Date of sale |

## Repository Structure

```text
advanced-sql-assignment/
│
├── README.md
├── sql/
│   ├── 01_dataset.sql
│   ├── 02_cte_revenue.sql
│   ├── 03_category_summary_view.sql
│   ├── 04_updatable_product_view.sql
│   ├── 05_products_by_category_procedure.sql
│   └── 06_product_archive_trigger.sql
│
├── answers/
│   └── assignment_answers.md
│
└── screenshots/
