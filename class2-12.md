## Reading Notes 12

## Status Codes Based On REST Methods

### In your own words, describe what each group of status code represents:

100’s = status code 100 - 199 informs the cliet "hat the header part of the request has been received [^1]", and that the server will continue with the request.

200's = status code 200-299 is an 'OK' or successful codes [^1]. It informs the client that their request has been accepted. The 202 asynchronous status code means that the request "met all validation requirements at the time of sending [^1]".

300’s = status code 300-399 are redirection codes. It informs the client whether the resource is not available anymore [^1].

400’s = status code 400-499 are client error codes, these are invalid request sent to a server [^1].

500’s = status code 500-599 are server error codes that can be temporary or permanent; it " indicate problems with overwhelmed servers or unreachable servers behind proxies", butclient requests can sometimes trigger the error exceptions on the server [^1].

### What is a status code 202?

The status code 202 is an asynchronous processing of request, it may not mean the request is processeed successfully, but it met all the requirements at the time of sending [^1].

### What does app.use(express.json()) do?

The express.json() is a "built-in middleware function in Express","used to parse the incoming requests with JSON payloads [^2]". The app.use([path], callback, [callback]) "method mounts or puts the specified middleware functions at the specified path [3]".

### What does the /:id mean in a route?




[^1]: [Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
[^2]: [Express.js – express.json() function](https://www.tutorialspoint.com/express-js-express-json-function#:~:text=json()%20is%20a%20built,header%20matches%20the%20type%20option.)
[^3]: [Express.js – app.use() Method]()](https://www.tutorialspoint.com/express-js-app-use-method)

