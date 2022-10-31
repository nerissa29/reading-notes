## Reading Notes 11

## nosql vs sql

### Fill in the chart below with five differences between SQL and NoSQL databases:

***SQL***, as explained through the article [^1]; [SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool) 

- known as RElational Database (RDBMS)
- is a table-based database; it represent data in form of tables
- has pre-defined schema
- uses *structured query language or SQL* for manipulating or defining the data
- are vertically scalable, increases the horse-power of the hardware


***NoSQL***, as explained through the article [^1]; [SQL vs NoSQL Database Differenc

- known as non-relational database
- are document based, key-value pairs, graph databases (or wide-column stores)
- has dynamic scheema 
- queries known as *unstructured query language or UnQL*, which focuses on document collection
- are horizontally , " scaled by increasing the databases servers in the pool of resources to reduce the load [^1]"



### What kind of data is a good fit for an SQL database?

According to the article [SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool), the SQL databases are good for complex queries; it is suited for storing structured data.

### Give a real world example.

Examples of data that can be stored and process using SQL are:

- zip codes
- city
- state
- dates
- ID numbers
- credit card numbers

Most relational databases support permission access, which means it defines who can read data and who is allowed to make changes on the data.


### What kind of data is a good fit for a NoSQL database?

Data with different forms or structures are good fit and easy to handle with NoSQL database [^2]. NoSQL can store and model data that are structured, semi-structured, or unstructured, in one database [^2]. It reduces "the need for translation from the form the data is stored in to the form the data takes in the code" - from [When to Use a NoSQL Database](https://www.mongodb.com/nosql-explained/when-to-use-nosql#:~:text=The%20structure%20of%20many%20different,unstructured%20data%20in%20one%20database.).


### Give a real world example.

It allows the developers "o be in control of the structure of the data"; "they are a good fit with modern Agile development practices based on sprints, quick iterations, and frequent code pushes [^2]". 

### Which type of database is best for hierarchical data storage?

NoSQL database are better for *hierarchical data storage* as it follows or uses the key-value pair when storing data, similar to JSON [^1].

### Which type of database is best for scalability?

Scalability in SQL (vertically scallable)can be managed by increasing the RAM, CPU, or SSD on one server, while NoSQL (horizintally scallable), can easily add servers "to handle the large traffic [^1]".


## sql vs nosql (Video)

### What does SQL stand for?

SQL stands for *Structured Query Language*.

### What is a relational database?

A relational database is a database that supports the SQL language [^4]. It is a database that "stores and provides access to data points that are related to one another [^4]". The data is stored and distributed across are then connected through relations; the sql can query these relations through some commands (ex. join) which can rerieve these connected data [^4].


### What type of structure does a relational database work with?

The relational databse supports data structures like forms, table data, data views and indexes. It supoorts logical data structures [^4]. It organizes and provids access to data points which makes it easier to access.

### What is a ‘schema’?

The *schema* refers to as a database organization or structure.

### What is a NoSQL database? How does it work?

NoSQL are document based, it stores data as key-value pairs, graph databases (or wide-column stores) [^1]. It is best fit for hierarchical data storage.

### What is inside of a MongoDB database?



[^1]; [SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool) 
[^2]: [When to Use a NoSQL Database](https://www.mongodb.com/nosql-explained/when-to-use-nosql#:~:text=The%20structure%20of%20many%20different,unstructured%20data%20in%20one%20database.)
[^3] [SQL vs NoSQL or MySQL vs MongoDB](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
[^4]: [What is a Relational Database (RDBMS)?](https://www.oracle.com/database/what-is-a-relational-database/)

