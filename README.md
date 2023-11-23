# Structured Query Language (SQL)

SELECT column_name(s) FROM table_name

##### * is used to select all columns

##### RECORD A record is a row of data, and a FIELD is a column of data

```sql
SELECT * FROM Customers;
```

```sql
# will print the column names with the data
SELECT CustomerName, City FROM Customers;
```


## Relational Databases
The different tables are related to each other by a common column. This allows us to connect the information in the different tables.

The columns fields are called KEYS


## Debugging

Databases won’t understand your queries if your SQL code contains mistakes and they will return an error message.

Errors in computer code are known as bugs and you’ll learn to identify and fix errors in this lesson.

Knowing how data is organized in the database will help you reduce errors.

A schema is a visual representation of how a database is organized, showing its tables, fields and keys. Arrows are used to show how the different tables are related.

A schema shows the fields a table contains. It doesn't show data values.

```sql
SELECT COLUMN_NAME(1), COLUMN_NAME(2) 
FROM TABLE_NAME
```

## SQL Comments
Single line comments
```sql
-- This is a comment
```

Multi line comments
```sql
/* This is a comment
that spans multiple lines */
```


## Sorting With SQL

Sorting means arranging the results so they are ordered in a meaningful way.

The ORDER BY keyword is used to sort the results in ascending or descending order.

```sql
SELECT column_name(s)
FROM table_name


ORDER BY column_name(s) ASC|DESC -- ASC is default
-- ASC is ascending order
-- DESC is descending order
```

### LIMIT
The LIMIT keyword is used to limit the number of results returned.

```sql
SELECT column_name(s)
FROM table_name
LIMIT 2
```

output:
```sql
id | column_name2 | column_name3
-------------------------------------------
1  | value2       | value3
2  | value2       | value3

```

#### OFFSET
The OFFSET keyword is used to offset the number of results returned.

```sql
SELECT column_name(s)
FROM table_name
LIMIT 2 OFFSET 2
```
output:
```sql
id | column_name2 | column_name3
-------------------------------------------
3  | value2       | value3
4  | value2       | value3

```

### AS 










