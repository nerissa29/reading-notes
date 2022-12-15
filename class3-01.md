## Reading Notes: SQL and Relational Database

### SQL Lesson 1: SELECT queries 101

**SELECT** is used to retrieve data from SQL database[^1]. ***SELECT*** statements are often referred to as ***queries***.

Example:

SELECT last_name FROM students

To retrieve all data from a table:

SELECT * FROM students

***Exercise 1:***

<img width="546" alt="image" src="https://user-images.githubusercontent.com/113204667/207411556-ebaed0de-324c-42e8-8499-11a50ad07ec7.png">

<img width="574" alt="image" src="https://user-images.githubusercontent.com/113204667/207411677-0a755898-43e6-445c-86d3-8be1557aec18.png">

<img width="574" alt="image" src="https://user-images.githubusercontent.com/113204667/207411771-22c27f71-5c54-4bc5-8375-9c529318ccba.png">

<img width="575" alt="image" src="https://user-images.githubusercontent.com/113204667/207411870-bf27c389-8368-4cdc-9e33-a9b1249ed71b.png">

<img width="564" alt="image" src="https://user-images.githubusercontent.com/113204667/207411959-be1a3879-d9b3-4887-bc5d-0bd095162090.png">


### SQL Lesson 2: Queries with constraints (Pt. 1)

The **WHERE** clause filters the data/results; it is "applied to each row of data by checking specific column values to determine whether it should be included in the results or not[^2]". 

The **AND** or **OR** can also be used to join more complex clauses.

Below is a screenshot of some useful operators from [SQL Lesson 2: Queries with constraints (Pt. 1)](https://sqlbolt.com/lesson/select_queries_with_constraints):

<img width="559" alt="image" src="https://user-images.githubusercontent.com/113204667/207415484-5b127a14-026c-4f36-8b13-60255c385d4b.png">

When there are hundreds or millions of rows of data, using clauses to constrain a set of data enables the query to run faster[^2].

***Exercise 2:***

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207416693-9de6daab-f8d5-429d-8c05-948b59e6409c.png">

<img width="593" alt="image" src="https://user-images.githubusercontent.com/113204667/207416948-2c266662-979d-4feb-ba1f-fec76ce8bea3.png">

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207417191-dbb4f70e-cce7-40ca-a5f3-4d50adf4905b.png">

<img width="592" alt="image" src="https://user-images.githubusercontent.com/113204667/207417613-4113c39b-b21a-4266-b8b2-bed85123dc52.png">


### SQL Lesson 3: Queries with constraints (Pt. 2)

Below is the screenshot from [SQL Lesson 3: Queries with constraints (Pt. 2)](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2), showing various useful operators that can be used in a (a) string comparison, and (b) wildcard pattern matching[^3]:

<img width="565" alt="image" src="https://user-images.githubusercontent.com/113204667/207418586-bdd5a74a-a870-454d-bb0f-fd836deb3c48.png">

"*All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords*[^3]."


***Exercise 3:***

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207420097-c72c0e57-1c54-46f2-95bd-8e244473b5a1.png">

<img width="587" alt="image" src="https://user-images.githubusercontent.com/113204667/207420319-f82c251f-bb67-4bfe-857d-b8a0f0b0368b.png">

<img width="589" alt="image" src="https://user-images.githubusercontent.com/113204667/207420418-723c6934-57c3-42f1-8272-e08d902b7f12.png">

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207420599-a5914c1f-c302-4950-8a88-cb92428e5bf7.png">


### SQL Lesson 4: Filtering and sorting Query results

The **DISTINCT** keyword is used to discard/remove rows with column values that are duplicates, while the **GROUP BY** clause is sued to discard duplicates on a specific column[^4].

The **ORDER BY** clause is used to sort results "by a given column in ascending or descending order[^4]".

An example from [SQL Lesson 4: Filtering and sorting Query results](https://sqlbolt.com/lesson/filtering_sorting_query_results):

```
Select query with ordered results
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```
Rows are sorted alpha-numerical based on the column's value when the clause **ORDER BY** is used. **LIMIT** and **OFFSET** are other clauses that can be used along with the **ORDER BY**. The **LIMIT** clause reduces the number of rows, while the **OFFSET** (optional) specifies where to start counting the number of rows from[^4].

An example from [SQL Lesson 4: Filtering and sorting Query results](https://sqlbolt.com/lesson/filtering_sorting_query_results):

```
Select a query with limited rows
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;

```

***Exercise 4:***

<img width="592" alt="image" src="https://user-images.githubusercontent.com/113204667/207427454-e9c691bf-c9f0-48c8-a452-4d09e59b4852.png">

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207428087-fd3a9c01-706d-45d8-b463-0d82ad1f5ce2.png">

<img width="587" alt="image" src="https://user-images.githubusercontent.com/113204667/207428225-4bf41458-bc74-4bb7-b794-b878095299fa.png">

<img width="587" alt="image" src="https://user-images.githubusercontent.com/113204667/207428488-e92fe503-4b11-4477-9621-87b29ed66e2f.png">


### SQL Lesson 5 (SQL Review): Simple SELECT Queries

***Review 1:***

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207432735-278f2cef-4d0a-44b5-8114-e71844a708b8.png">

<img width="589" alt="image" src="https://user-images.githubusercontent.com/113204667/207433148-9846da14-72cc-4096-aaef-e9ecd766142b.png">

<img width="561" alt="image" src="https://user-images.githubusercontent.com/113204667/207434385-44720e6e-34da-43e9-82d6-f218446e2921.png">

<img width="591" alt="imagez" src="https://user-images.githubusercontent.com/113204667/207434928-ce60c039-01a7-42d8-9b74-de515f135457.png">

<img width="590" alt="image" src="https://user-images.githubusercontent.com/113204667/207435527-f5371387-f42a-4a01-b427-b23965e2a6c0.png">


### SQL Lesson 6: Multi-table queries with JOINs

A *primary key* is needed to uniquely identify the data across the database; a primary key can be a string or hashed value, but it can also be an auto-incrementing integer[^5]. Combining the data from different parts of the database is possible using the **JOIN** clause. The *JOIN* clause combines data in a row "across two separate tables using this unique key[^5]".

The **INNER JOIN** is one of the JOIN clauses; it " is a process that matches rows from the first table and the second table which have the same key (as defined by the ON constraint) to create a result row with the combined columns from both tables", as stated in [SQL Lesson 6: Multi-table queries with JOINs](https://sqlbolt.com/lesson/select_queries_with_joins). Once they're joined, other clauses learned can be used to query data to return the information needed.


***Exercise 6:***

<img width="592" alt="image" src="https://user-images.githubusercontent.com/113204667/207688117-9dec16f0-6809-408f-acae-eae48b99f22e.png">

<img width="593" alt="image" src="https://user-images.githubusercontent.com/113204667/207690027-682eb2c1-5588-4c12-8ecb-3a0d82ed7e65.png">

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207691219-e5a0ed3f-a89a-44b2-835c-7eb0a6b2c567.png">

## Lessons 13 through 18 - Database Management

### SQL Lesson 13: Inserting rows

A "table in a database is a two-dimensional set of rows and columns, with the columns being the properties and the rows being instances of the entity in the table", as described from [SQL Lesson 13: Inserting rows](https://sqlbolt.com/lesson/inserting_rows), while the **database schema** describes the table structure and the datatypes from its column[^6].

When inserting new data, the **INSERT** statement is used; it describes which table to write (ex., INSERT INTO movies)[^6]. When adding data to a database, the row must contain values for each table column.

Below are the examples provided from [SQL Lesson 13: Inserting rows](https://sqlbolt.com/lesson/inserting_rows):

```
Insert statement with values for all columns
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
       
```

```
Insert statement with specific columns
INSERT INTO mytable
(column, another_column, …)
VALUES (value_or_expr, another_value_or_expr, …),
      (value_or_expr_2, another_value_or_expr_2, …),
      …;
      
```
The first example above allows inserting of multiple rows by "listing them sequentially[^6]". In contrast, the second example allows to insert data/rows "with only the columns of data you have by specifying them explicitly[^6]".

***Exercise 13:***

<img width="593" alt="image" src="https://user-images.githubusercontent.com/113204667/207700780-51ad11cf-1fea-4c3b-853a-b57c375b5f59.png">

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207701192-fd565b8c-2578-43d3-bcf0-581b4cd77bd6.png">

### SQL Lesson 14: Updating rows

Another common task in database management is updating the existing data. In updating rows, the **UPDATE** statement specifies the table, columns, and rows that need updating [^7]. Like INSERT, in UPDATE, the data "has to match the data type of the columns in the table schema", as stated in [SQL Lesson 14: Updating rows](https://sqlbolt.com/lesson/updating_rows).

UPDATE statement example below from [SQL Lesson 14: Updating rows](https://sqlbolt.com/lesson/updating_rows):

```
Update statement with values
UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;

```
The **WHERE** clause is necessary as it states the condition or where to apply the update. It is a good practice to always "write the constraint first and test it in a SELECT query to make sure you are updating the right rows, and only then write the column/value pairs to update[^7]".

***Exercise 14:***

<img width="595" alt="image" src="https://user-images.githubusercontent.com/113204667/207703576-3620d677-9254-4fc9-8dc9-5576723fe81b.png">

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207703936-9b764c01-8d86-4dd2-9bfe-16ddfe901654.png">

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207704539-514114e8-2819-45c0-858a-f23d1ca9cd63.png">


### SQL Lesson 15: Deleting rows

A **DELETE** statement is used when needed to delete rows; the delete statement goes like this:  **DELETE FROM** *table_name* **WHERE** *condition*[^8], as shown below.

An example from [SQL Lesson 15: Deleting rows](https://sqlbolt.com/lesson/deleting_rows):

```
Delete statement with condition
DELETE FROM mytable
WHERE condition;

```

Without the **WHERE** clause, all rows will be deleted; it is why the **WHERE** clause is important to both the UPDATE and DELETE statements. It is advised to always double-check the DELETE statement before executing it.


***Exercise 15:***

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207720657-c25e9e4e-4f3a-46d8-b697-579c750964a3.png">

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207720975-2bbb2422-1ec6-4aad-a77b-bb3c428e029d.png">


### SQL Lesson 16: Creating tables

The **CREATE TABLE** statement is used to create a new database - new entities and new relationships[^9].

An example below is provided from [SQL Lesson 16: Creating tables](https://sqlbolt.com/lesson/creating_tables):

```
Create table statement w/ optional table constraint and default value
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);

```

The new table's structure is defined by its **table schema**, which defines its columns, including its name, data type, and constraint if needed[^9]. The **IF NOT EXISTS** clausee is used to skip creating table if table with the same name already exists[^9]. By default, SQL will throw an error if creating a table with a name that already exists.

Below is the screenshot of data types from [SQL Lesson 16: Creating tables](https://sqlbolt.com/lesson/creating_tables):

<img width="540" alt="image" src="https://user-images.githubusercontent.com/113204667/207740875-5128330c-840e-41a5-9f3e-b056d92c25d8.png">


Below is the screenshot of table constraints from [SQL Lesson 16: Creating tables](https://sqlbolt.com/lesson/creating_tables):

<img width="544" alt="image" src="https://user-images.githubusercontent.com/113204667/207740942-f33fa261-c2c4-4080-890f-e319a1eee7cf.png">


Below is a CREATE TABLE statement example from [SQL Lesson 16: Creating tables](https://sqlbolt.com/lesson/creating_tables):

```
Movies table schema
CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER, 
    length_minutes INTEGER
);

```

***Exercise 16:***

<img width="589" alt="image" src="https://user-images.githubusercontent.com/113204667/207741523-a93859eb-863e-4960-916f-1a53daea0468.png">


### SQL Lesson 17: Altering tables

The **ALTER TABLE** statement allows to add, remove, update or modify the columns and table constraints in the database[^10]. Below are the syntax for altering the table (adding, removing, and renaming the table), as stated in [SQL Lesson 17: Altering tables](https://sqlbolt.com/lesson/altering_tables):

*Adding Columns*
```
Altering table to add new column(s)
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
    
```

*Removing Columns*
```
Altering table to remove column(s)
ALTER TABLE mytable
DROP column_to_be_deleted;

```

*Renaming the table*
```
Altering table name
ALTER TABLE mytable
RENAME TO new_table_name;

```

***Exercise 17:***




References:
[^1]: [SQL Lesson 1: SELECT queries 101](https://sqlbolt.com/lesson/select_queries_introduction)
[^2]: [SQL Lesson 2: Queries with constraints (Pt. 1)](https://sqlbolt.com/lesson/select_queries_with_constraints)
[^3]: [SQL Lesson 3: Queries with constraints (Pt. 2)](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2)
[^4]: [SQL Lesson 4: Filtering and sorting Query results](https://sqlbolt.com/lesson/filtering_sorting_query_results)
[^5]: [SQL Lesson 6: Multi-table queries with JOINs](https://sqlbolt.com/lesson/select_queries_with_joins)
[^6]: [SQL Lesson 13: Inserting rows](https://sqlbolt.com/lesson/inserting_rows)
[^7]: [SQL Lesson 14: Updating rows](https://sqlbolt.com/lesson/updating_rows)
[^8]: [SQL Lesson 15: Deleting rows](https://sqlbolt.com/lesson/deleting_rows)
[^9]: [SQL Lesson 16: Creating tables](https://sqlbolt.com/lesson/creating_tables)
[^10]: [SQL Lesson 17: Altering tables](https://sqlbolt.com/lesson/altering_tables)






