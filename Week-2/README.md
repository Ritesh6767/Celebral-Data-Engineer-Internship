# Week 2 SQL Assignment

This folder contains the SQL assignment for Week 2, which explores basic database design, querying, joins, aggregation, and transaction concepts using SQLite.

## Files included

- `sql-assignment.ipynb` — a Jupyter notebook that builds the database schema, inserts sample data, and runs the SQL queries for each section.
- `celebral.db` — the SQLite database file used by the notebook.
- `Sample - Superstore.csv` — a dataset included in the folder, though the main work for this assignment is done in the notebook.

## What the notebook covers

The assignment is organized in several sections:

1. **Schema and constraints**
   - Creates four tables: `customers`, `products`, `orders`, and `order_items`
   - Demonstrates primary keys, foreign keys, UNIQUE, NOT NULL, CHECK constraints, and indexes
   - Inserts example data for customers, products, orders, and order items

2. **Filtering and optimization**
   - Uses `WHERE` clauses to filter orders and products
   - Shows how indexes help with date-based queries
   - Explains why functions on indexed columns can prevent index usage

3. **Aggregation**
   - Uses `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`
   - Groups order data by status to calculate revenue and order counts
   - Computes average order value and total revenue for delivered orders

4. **Joins and relationships**
   - Demonstrates `INNER JOIN`, `LEFT JOIN`, and multi-table joins
   - Explains the foreign key relationships between tables
   - Shows how to join orders with customers and order items with products

5. **Advanced concepts**
   - Uses `CASE` expressions to categorize products by price tier
   - Explains ACID properties and shows a sample transaction block with `BEGIN`, `COMMIT`, and rollback behavior

## How to run

1. Open `sql-assignment.ipynb` in Jupyter Notebook or JupyterLab.
2. Run the notebook cells in order.
3. The notebook uses `%sql sqlite:///celebral.db` to connect to the local SQLite database.

## Notes

- The notebook includes some explanatory answers written alongside the SQL queries.
- Most of the queries are written in standard SQL and should work in SQLite with minor adjustments if run in another SQL environment.
- The sample data is intentionally small and structured to support the assignment questions.

---

If you want to inspect the database directly, open `celebral.db` with any SQLite viewer or use the notebook again to query additional data.