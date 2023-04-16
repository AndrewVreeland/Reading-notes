# [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/[])

1. In your own words, describe what each group of status code represents:
      * 100’s = informational status codes, will tell the user that the request has been recieved and server will try to comply with request.
      * 200’s = success codes
      * 300’s = redirection codes resource isnt available at the expected location.
      * 400’s = client error codes invalid request sent to the server
      * 500’s = server error codes problems with overhwelmed servers, temporary or permanent.
2. What is a status code 202?
      * async processing request. the request met all validation requirements before sending.
3. What is a status code 308?
      * tells the client to use another URL to access the resource and not use the current url anymore
4. What code would you use if an update didn’t return data to a client?
      * 204 NO CONTENT
5. What code would you use if a resource used to exist but no longer does?
      * 410 GONE
6. What is the ‘Forbidden’ status code?
      * 403 Forbidden: The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Videos

[Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
      * We need to put our MongoDB database string into a .env file or an environment variable for security reasons.
2. What is middleware?
      * Middleware is a term used to describe software components that are designed to handle requests and responses in a web application or API. In the context of web development, middleware is a software layer that sits between the client and the server, and can intercept and modify requests and responses as they pass through.
3. What does app.use(express.json()) do?
      * is a middleware function in the Express.js framework for Node.js. It is used to parse incoming JSON payloads in request bodies.

When a client sends a JSON payload to a server, the payload is usually included in the body of a POST, PUT, or PATCH request. In order for the server to work with this data, it needs to be parsed from a string into a JavaScript object that can be used in server-side code. This is where express.json() comes in.
4. What does the /:id mean in a route?
      * The : in front of id indicates that it is a parameter. This means that the value for id can be different each time the route is called. For example, a route definition like /users/:id would match requests for URLs like /users/123, /users/456, and so on.
5. What is the difference between PUT and PATCH?
      * The main difference between PUT and PATCH is the level of granularity they offer for updates. PUT is used to completely replace an existing resource with a new one, while PATCH is used to partially update an existing resource.
6. How do you make a default value in a schema?
      * In Mongoose, you can define default values for a schema field using the default option when defining the schema. default: 0
7. What does a 500 error status code mean?
        * A 500 Internal Server Error status code is a generic HTTP status code that indicates that an unexpected error occurred on the server while processing a request. This error status code is usually sent by the server when it encounters an error that prevents it from fulfilling the request made by the client.
8. What is the difference between a status 200 and a status 201?
      * a status code of 200 indicates that the request has succeeded, while a status code of 201 indicates that the request has succeeded and a new resource has been created on the server.