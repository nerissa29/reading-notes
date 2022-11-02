## Reading Notes 13

### CRUD Basics

#### Which HTTP method would you use to update a record through an API?

To update something, the HTTP PUT method is used. This method will replace the current data of the target with the new content [^1].

### Which REST methods require an ID parameter?

The *DELETE* and *PUT* method grabs/requires the id of the target resource that needs to be deleted o updated. A unique identifier is necessary to remove or change a specific resource.

## Speed Coding: Building a CRUD API

### What’s the relationship between REST and CRUD?

CRUD stands for *Create, Read, Update, and Delete*; it describes the four essential functions "that models should be able to do and are considered necessary to implement a persistent storage application [^1]". The four basic functions it represents are *create, read, update, and delete*, which corresponds to *post, get, put, and delete* in HTTP/REST methods. CRUD is a function that can live within REST; REST is a standard API architecture.

### If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

- Bring in all the required libraries and routers required
- require the model, connect to the database, create middleware
- create endpoints and parameters needed, as well as create async functions needed
- handle errors
- Export the router/model

.
[^1]: [CRUD Operations Explained](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)
