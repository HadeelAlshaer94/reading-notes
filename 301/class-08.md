# Code 301 - Intermediate Software Development

# APIs and REST 
REST stands for representational state transfer and was created by computer scientist Roy Fielding.
![rest](https://www.abbreviations.com/images/363406_REST.png)

## REST APIs are designed around a resources.
which are any kind of object, data, or service that can be accessed by the client.

## A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

https://adventure-works.com/orders/1

## What are the most common HTTP verbs?
The most common operations are GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on?
resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI.
https://adventure-works.com/orders // Good

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?(BAD)
Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.

## (GET) A successful GET method typically returns HTTP status code 200 (OK). If the resource cannot be found, the method should return 404 (Not Found).

## (POST) If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body. Alternatively, if there is no result to return, the method can return HTTP status code 204 (No Content) with no response body.

If the client puts invalid data into the request, the server should return HTTP status code 400 (Bad Request). The response body can contain additional information about the error or a link to a URI that provides more details.

## (DELETE) If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled, but that the response body contains no further information. If the resource doesn't exist, the web server can return HTTP 404 (Not Found).