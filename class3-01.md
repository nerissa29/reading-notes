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


References:
[^1]: [SQL Lesson 1: SELECT queries 101](https://sqlbolt.com/lesson/select_queries_introduction)
[^2]: [SQL Lesson 2: Queries with constraints (Pt. 1)](https://sqlbolt.com/lesson/select_queries_with_constraints)
[^3]: [SQL Lesson 3: Queries with constraints (Pt. 2)](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2)
[^4]: [SQL Lesson 4: Filtering and sorting Query results](https://sqlbolt.com/lesson/filtering_sorting_query_results)
[^5]: [SQL Lesson 6: Multi-table queries with JOINs](https://sqlbolt.com/lesson/select_queries_with_joins)

