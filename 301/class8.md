# README.md

## Read Assignment 8

1.REST stands for Representational State Transfer

2.REST APIs are designed around resources.

3.the resource identifier is known as URI. It uniquely identifies the resource.

4.GET, POST, PUT, PATCH, and DELETE are the most common HTTP verbs.

5.URIs should be based on the resource (or nouns) instead of verbs (or the operations).

6.here shouldn't be trailing '/' in URIs; it must be only used to indicate the hierarchical relationship. Hyphens are used to improve the URIs readability, while underscores should not be used. The URI paths should be in lowercase letters, as preferred, and no file extensions should be included.

7.Chatty web APIs can "expose a large number of small resources 1Links to an external site.". It might require multiple requests/calls to find data, combining it into more extensive resources, which can be done in a single request. These numerous requests might slow down the app.

8.The GET is used to retrieve data/resources specified at URI

9.It returns status code 404, which is a Not Found. If the request is fulfilled, but there are no contents to produce, status code 204 No Content must be returned

10.f the POST method successfully creates a new resource, a status code 201 Created is returned. In the location header of the response, the "URI of the new resource is included

11.A successful DELETE method returns a status code 204 No Content, which indicates that the process is successful and that the response body does not have the data anymore
