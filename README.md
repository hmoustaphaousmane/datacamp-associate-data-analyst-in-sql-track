# datacamp-associate-data-analyst-in-sql-track

This repository contains my projects and submissions for DataCamp's Associate Data Analyst in SQL track.

## Intoduction to SQL

SQL stands for Structured Query Language. It is aprogramming language used to manage and manipulate data stored in relational databases. In relational databases, data are stored in tables (relations). A table is consisted of rows (records) and columns (fields) and have relatuons with other tables.
In SQL, there are four main data types:
	- numeric type: NUMERIC, INTEGER, FLOAT ...
	- character type: CHAR, VARCHAR, TEXT
	- datetime types: DATE, TIME, TIMESTAMP
	- boolean: TRUE, FALSE.
As mentioned before, SQL is used to manage relational databases. So, let's see some SQL basic commands:
- database creation:

```sql
CREATE DATABASE db_name;
```

- create a table:

```sql
CREATE TABLE table_name(
  column1 datatype,
  column2 datatype,
  ...
)
```

Or

```sql
CREATE TABLE table_name();

ALTER TABLE table_name ADD COLUMN column_name datatype;
-- repeat for each column
```

- retrieve data from a table

```sql
SELECT column1, column2
FROM table_name;

-- to select all fields of a table
SELECT *
FROM tabla_name;
```

- add new records to a table

```sql
INSERT INTO table_name(column1, column2) VALUES(value1, value2);
```

- update existing record

```sql
UPDATE table_name
SET column1 = newvalue1, column2 = newvalue2
WHERE condition;
```

- delete a record

```sql
DELETE FROM table_name
WHERE condition;
```

- delete a table

```sql
DROP TABLE table_name;
```

- delete a database

```sql
DROP DATABASE database_name;
```

- create a view

A view is a virtual table that is based on the result of a `SELECT` query.

```sql
CREATE VIEW view_name AS
SELECT columns
FROM table
WHERE condition;
```

A view is queried just like a regular table

```sql
SELECT columns
FROM view_name;
```

