# MovieCo Rental Database: SQL Analysis

A relational database and set of analytical T-SQL queries for a movie rental business, built in SQL Server Management Studio (SSMS) as part of my M.S. in Business Analytics coursework at Suffolk University.

## What it covers
- **Schema design:** six normalized tables (`PRICE`, `MOVIE`, `VIDEO`, `MEMBERSHIP`, `RENTAL`, `DETAILRENTAL`) with primary keys, a composite key on `DETAILRENTAL`, and foreign keys enforcing every relationship.
- **Analytical queries:**
  1. Rental transactions above average in both video count and total fee (`GROUP BY` + `HAVING` with subqueries)
  2. Longest rental duration for returned videos (CTE + `DATEDIFF`)
  3. Members with above-average rental income, handling NULL late fees (CTE + `ISNULL`)
  4. Top genres by rental income, count and average fee (`TOP`, aggregation), to support pricing decisions

## Skills demonstrated
`JOIN`s across 5 tables, CTEs, subqueries, aggregation, `HAVING`, NULL handling, date arithmetic, DDL with constraints.

## Files
| File | Description |
|---|---|
| `schema.sql` | `CREATE TABLE` statements in dependency order |
| `queries.sql` | The four analysis queries |

## How to run
1. Open SSMS and create or select a database.
2. Run `schema.sql`.
3. Load your own sample data (rows for each table).
4. Run the queries in `queries.sql`.

## Tech
SQL Server (T-SQL), SSMS
