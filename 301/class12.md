# README.md

## Read Assignment 12

1.100’s = status code 100 - 199 informs the client hat the header part of the request has been received and that the server will continue.

200's = status code 200-299 informs the client that their request has been accepted. The 202 asynchronous status code means that the request met all validation requirements at the time of sending .

300’s = status codes 300-399 are redirection codes. informs the client whether the resource is not available anymore.

400’s = status code 400-499 are client error codes; these are invalid requests sent to a server 1.

500’s = status codes 500-599 are server error codes that can be temporary or permanent; they indicate problems with overwhelmed servers or unreachable servers behind proxies, but client requests can sometimes trigger the error exceptions on the server.

2.The status code 202 is an asynchronous processing of the request, it may not mean the request is processed successfully, but it met all the requirements at the time of sending.

3.308 is a permanent redirect status response code that indicates that the resource requested has been definitively moved to the URL given by the Location headers.

4.If the server has fulfilled the request, but there is no need to return data, it must send a 204 (No Content) status code

5.If the server cannot find anything matching the client's request, a 404 status must be used. The status code 410 (Gone) should be used only if the server knows that an old resource is no longer available or has no forwarding address.

6.The status code 403 is a Forbidden status code, which means that the server understands and knows the request but is refusing to complete it . The client may have authorized itself but still has no permissions to access the resource.

7.It is a connection used to join the MongoDB Database; without it, we won't be able to connect to the database server.

8.Middleware is functions that have access to the request or response objects, and the next middleware function in the application’s request-response cycle, which is noted by the word next.

9.The express.json() is a built-in middleware function in Express, used to parse the incoming requests with JSON payloads 4. The app.use([path], callback, [callback]) method mounts or puts the specified middleware functions at the specified path .

10.It is a URL segment or route parameter that captures the values specified in the URL position.

11.PUT is a method of changing the resources where the client sends data that updates the entire resource 6. At the same time, PATCH is a method of modifying/changing resources where the client sends partial data that is to be updated without modifying the entire data.

12.According to the article Mongoose: Defaults, if the path has no value or is undefined, the mongoose will apply the default value. If a new document without a path is created, the default values will kick in.

13.500 status code is a server error code; a problem prevented it from completing the request.

14. 201 status code means that the request has been completed, resulting in the creation of a new resource 2. The 200 status code indicates an 'OK' or successful request 12. It means that the request was received, accepted, and is being processed 12.
