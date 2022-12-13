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

Below is the screenshot from [SQL Lesson 3: Queries with constraints (Pt. 2)](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2), showing various useful operators that can be used in (a) string comparison, and (b) wildcard pattern matching[^3]:

<img width="565" alt="image" src="https://user-images.githubusercontent.com/113204667/207418586-bdd5a74a-a870-454d-bb0f-fd836deb3c48.png">

"*All strings must be quoted so that the query parser can distinguish words in the string from SQL keywords*[^3]"


***Exercise 3:***

<img width="591" alt="image" src="https://user-images.githubusercontent.com/113204667/207420097-c72c0e57-1c54-46f2-95bd-8e244473b5a1.png">

<img width="587" alt="image" src="https://user-images.githubusercontent.com/113204667/207420319-f82c251f-bb67-4bfe-857d-b8a0f0b0368b.png">

<img width="589" alt="image" src="https://user-images.githubusercontent.com/113204667/207420418-723c6934-57c3-42f1-8272-e08d902b7f12.png">

<img width="588" alt="image" src="https://user-images.githubusercontent.com/113204667/207420599-a5914c1f-c302-4950-8a88-cb92428e5bf7.png">


### SQL Lesson 4: Filtering and sorting Query results



References:
[^1]: [SQL Lesson 1: SELECT queries 101](https://sqlbolt.com/lesson/select_queries_introduction)
[^2]: [SQL Lesson 2: Queries with constraints (Pt. 1)](https://sqlbolt.com/lesson/select_queries_with_constraints)
[^3]: [SQL Lesson 3: Queries with constraints (Pt. 2)](https://sqlbolt.com/lesson/select_queries_with_constraints_pt_2)
[^4]: [SQL Lesson 4: Filtering and sorting Query results](https://sqlbolt.com/lesson/filtering_sorting_query_results)

