## Reading 08

## API Design Best Practices

### What does REST stand for?

REST stands for Representational State Transfer; It is an architectural approach in design web pes [^1]. Roy Fielding proposed it in 2000. REST is not tied to HTTP, but most of its implementations use HTTP as the application protocol [^1].

### REST APIs are designed around a ____.

REST APIs are designed around resources.

### What is an identifier of a resource? Give an example.

According to the document [RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest), the resource identifier is known as *URI*. It uniquely identifies the resource.

### What are the most common HTTP verbs?

*GET, POST, PUT, PATCH, and DELETE* are the most common HTTP verbs. These verbs "perform operations on resources [^1]".

### What should the URIs be based on?

The article [RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest) states that the URIs should be based on the resource (or nouns) instead of verbs (or the operations).

### Give an example of a good URI.

*"http://api.canvas.com/shapes [^2]"*.

According to the article [RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest), there shouldn't be trailing '/' in URIs; it must be only used to indicate the hierarchical relationship. Hyphens are used to improve the URIs readability, while underscores should not be used. The URI paths should be in lowercase letters, as preferred, and no file extensions should be included [^2].

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

Chatty web APIs can "expose a large number of small resources [^1]". It might require multiple requests/calls to find data, combining it into more extensive resources, which can be done in a single request. These numerous requests might slow down the app.

### What status code does a successful GET request return?

The GET is used to retrieve data/resources specified at URI. The response message "contains the details of the requested resource [^1]".

### What status code does an unsuccessful GET request return?

According to the article [RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest), it returns status code 404, which is a *Not Found*. If the request is fulfilled, but there are no contents to produce, status code 204 *No Content* must be returned [^1].

### What status code does a successful POST request return?

If the *POST method* successfully creates a new resource, a status code 201 *Created* is returned. In the location header of the response, the "URI of the new resource is included [^1]".

### What status code does a successful DELETE request return?

A successful *DELETE method* returns a status code 204 *No Content*, which indicates that the process is successful and that the response body does not have the data anymore [^1].



[^1]: [RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design#what-is-rest)
[^2]: [7 Rules for REST API URI Design](https://blog.restcase.com/7-rules-for-rest-api-uri-design/)
