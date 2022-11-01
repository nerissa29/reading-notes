## Reading Notes 12

## Status Codes Based on REST Methods

### In your own words, describe what each group of status code represents:

100’s = status code 100 - 199 informs the client "that the header part of the request has been received [^1]" and that the server will continue.

200's = status code 200-299 is an ‘OK’ or successful code [^1]. It informs the client that their request has been accepted. The 202 asynchronous status code means that the request "met all validation requirements at the time of sending [^1]".

300’s = status codes 300-399 are redirection codes. It informs the client whether the resource is not available anymore [^1].

400’s = status code 400-499 are client error codes; these are invalid requests sent to a server [^1].

500’s = status codes 500-599 are server error codes that can be temporary or permanent; they" indicate problems with overwhelmed servers or unreachable servers behind proxies,” but client requests can sometimes trigger the error exceptions on the server [^1].

### What is a status code 202?

The status code 202 is an asynchronous processing of the request, it may not mean the request is processed successfully, but it met all the requirements at the time of sending [^1].

### What is status code 308?

According to [MDN: 308 Permanent Redirect](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/308#:~:text=The%20HyperText%20Transfer%20Protocol%20(HTTP,given%20by%20the%20Location%20headers.), status code 308 is a *permanent redirect* status response code that indicates "that the resource requested has been definitively moved to the URL given by the Location headers.”  


### What code would you use if an update didn’t return data to a client?

If the server has fulfilled the request, but there is no need to return data, it must send a 204 (No Content) status code [^7].


### What code would you use if a resource used to exist but no longer does?

If the server cannot find anything matching the client's request, a 404 (Not Found) status must be used. The status code 410 (Gone) should be used only if the server knows that an old resource is no longer available or has no forwarding address [^7].

### What is the ‘Forbidden’ status code?

The status code 403 is a Forbidden status code, which means that the server understands and knows the request but is refusing to complete it [^7]. The client may have authorized itself but "still has no permissions to access the resource [^1]". 



## Build A REST API With Node.js, Express, & MongoDB - Quick -


### Why do we need to pull our MongoDB database string

It is a connection used to join the MongoDB Database; without it, we won't be able to connect to the database server.


### What is middleware?

Middleware is functions that have access to the request or response objects, "and the next middleware function in the application’s request-response cycle"[^8], which is noted by the word *next*.



### What does app.use(express.json()) do?

The express.json() is a "built-in middleware function in Express”, “used to parse the incoming requests with JSON payloads [^2]". The app.use([path], callback, [callback]) "method mounts or puts the specified middleware functions at the specified path [3]".

### What does the /:id mean in a route?

It is a URL segment or route parameter that captures the values specified in the URL position [^4].


### What is the difference between PUT and PATCH?

PUT is a method of changing the resources "where the client sends data that updates the entire resource [^5]". At the same time, PATCH is a method of modifying/changing resources "where the client sends partial data that is to be updated without modifying the entire data [^5]".

### How do you make a default value in a schema?

According to the article [Mongoose: Defaults](https://mongoosejs.com/docs/defaults.html), if the path has no value or is undefined, the mongoose will apply the default value. If a new document without a path is created, the default values will kick in.

### What does a 500 error status code mean?

The status code 500 is a server error code; a problem prevented it from completing the request [^1].

### What is the difference between a status 200 and a status 201?

The 201 status code means that the request has been completed, resulting in the creation of a new resource [^7]. The 200 status code indicates an 'OK' or successful request [^1][^7]. It means that the request was received, accepted, and is being processed [^1][^7].

[^1]: [Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
[^2]: [Express.js – express.json() function](https://www.tutorialspoint.com/express-js-express-json-function#:~:text=json()%20is%20a%20built,header%20matches%20the%20type%20option.)
[^3]: [Express.js – app.use() Method]()](https://www.tutorialspoint.com/express-js-app-use-method)
[^4]: [Express: Routing](https://expressjs.com/en/guide/routing.html)
[^5]: [Difference Between PUT and PATCH Request](https://www.geeksforgeeks.org/difference-between-put-and-patch-request/#:~:text=PUT%20is%20a%20method%20of%20modifying%20resource%20where%20the%20client,without%20modifying%20the%20entire%20data.)
[^6]: [Mongoose: Defaults](https://mongoosejs.com/docs/defaults.html)
[^7]: [Hypertext Transfer Protocol -- HTTP/1.1](https://www.rfc-editor.org/rfc/rfc2616#section-10.2.2)
[^8]: [Express: Using middleware[]()](https://expressjs.com/en/guide/using-middleware.html)

