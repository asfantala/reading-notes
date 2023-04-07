# Introduction to [SQL](https://sqlbolt.com/)

## What is SQL?
SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

## Popular SQL databases :
* SQLite
* MySQL
* Postgres
* Oracle 
* Microsoft SQL Server

## 1: SELECT queries
The most basic query we could write would be one that selects for a couple columns (properties) of the table with all the rows (instances)
```
SELECT column, another_column, … FROM mytable;
```
And  If we want to retrieve absolutely all the columns of data from a table
```
SELECT * FROM mytable;
```

##  2: Queries with constraints 
In order to filter certain results from being returned, we need to use a WHERE clause in the query
When writing WHERE clauses with columns containing text data, SQL supports a number of useful operators to do things like case-insensitive string comparison and wildcard pattern matching
```
SELECT column, another_column, … FROM mytable
 WHERE condition
    AND/OR another_condition
    AND/OR …;
```

##  3: Filtering and sorting Query results
SQL provides a convenient way to discard rows that have a duplicate column value by using the DISTINCT keyword.
```
SELECT DISTINCT column, … FROM mytable WHERE condition(s);
```

QL provides a way to sort your results by a given column in ascending or descending order using the ORDER BY clause.
```
SELECT column,... FROM mytable WHERE condition(s) ORDER BY column ASC/DESC;
```
Another clause which is commonly used with the ORDER BY clause are the LIMIT and OFFSET clauses, The LIMIT will reduce the number of rows to return, and the optional OFFSET will specify where to begin counting the number rows from

```
SELECT column,… FROM mytable WHERE condition(s) ORDER BY column ASC/DESC LIMIT num_limit OFFSET num_offset;
```

## 4: Multi-table queries with JOINs
The INNER JOIN is a process that matches rows from the first table and the second table which have the same key (as defined by the ON constraint) to create a result row with the combined columns from both tables.
```
SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
```
inner join might not be sufficient because the resulting table only contains data that belongs in both of the tables so we would have to use a LEFT JOIN, RIGHT JOIN or FULL JOIN instead to ensure that the data you need is not left out of the results.
```
SELECT column, another_column, …
FROM mytable
INNER/LEFT/RIGHT/FULL JOIN another_table 
    ON mytable.id = another_table.matching_id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;
```
## 5: A short note on NULLs

you will likely have to write additional logic to deal with NULLs in the result and constraints
```
SELECT column, another_column, …
FROM mytable
WHERE column IS/IS NOT NULL
AND/OR another_condition
AND/OR …;
```

## 6: Queries with expressions
```
SELECT col_expression AS expr_description, … FROM mytable;
```
## 7: Queries with aggregates
```
SELECT AGG_FUNC(column_or_expression) AS aggregate_description, …
FROM mytable
WHERE constraint_expression
```

SQL allows us to do this by adding an additional HAVING clause which is used specifically with the GROUP BY clause to allow us to filter grouped rows from the result set
```
SELECT group_by_column, AGG_FUNC(column_expression) AS aggregate_result_alias, …
FROM mytable
WHERE condition
GROUP BY column
HAVING group_condition;
```

## 8: Order of execution of a Query
```
SELECT DISTINCT column, AGG_FUNC(column_or_expression), …
FROM mytable
    JOIN another_table
      ON mytable.column = another_table.column
    WHERE constraint_expression
    GROUP BY column
    HAVING constraint_expression
    ORDER BY column ASC/DESC
    LIMIT count OFFSET COUNT;
```


## 9: Inserting rows

```
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
```

Insert statement with specific columns
```
INSERT INTO mytable
(column, another_column, …)
VALUES (value_or_expr, another_value_or_expr, …),
      (value_or_expr_2, another_value_or_expr_2, …),
      …;
```

## 10: Updating rows

```
UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;
```
## 11: Deleting rows
```
DELETE FROM mytable
WHERE condition;
```
## 12: Creating tables
```
Create table statement w/ optional table constraint and default value
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
```
Here's an example schema for the Movies table that we've been using Table data types.

```
CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER, 
    length_minutes INTEGER
);
```
## 13: Altering tables

ALTER TABLE statement to add, remove, or modify columns and table constraints.

### Adding columns

```
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
```
### Removing columns
```
ALTER TABLE mytable
DROP column_to_be_deleted;
Renaming the table
```
### If you need to rename the table itself, you can also do that using the RENAME TO clause of the statement.

```
ALTER TABLE mytable
RENAME TO new_table_name;
```

## 14: Dropping tables
 the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.
```
DROP TABLE IF EXISTS mytable;
```

![I have finished the cource ](./Capture.PNG)
