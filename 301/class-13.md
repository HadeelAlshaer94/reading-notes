# Code 301 - Intermediate Software Development

# CRUD
# Status Codes Based On REST Methods
## In your own words, describe what each group of status code represents:
- **100’s** = They usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

- **200’s** =  These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

- **300’s** =  These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

- **400’s** =  These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

- **500’s** =  These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

## What is a status code 202?
- **202 Accepted** - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

## What is a status code 308?
-**308 Permanent Redirect** - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. 

## What code would you use if an update didn’t return data to a client?
- **204 No Content**

## What code would you use if a resource used to exist but no longer does?
- **414 Request-URI Too Long**

## What is the ‘Forbidden’ status code?
- **403 Forbidden** - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

# Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

## What is middleware?
- Middleware is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

## What is the difference beween PUT and PATCH?
- **PUT** is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely.
- Unlike PUT, **PATCH** applies a partial update to the resource.
This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.

## How do you make a defalut value in a schema?
- Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

## What does a 500 error status code mean?
- 500 means Internal Server Error, which can be anything from a missing header field the backend accessed without checking its existence to an unreachable third party service the backend wanted to call.

## What is the difference between a status 200 and a status 201?
- **202 Accepted** - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.
- **201 Created** - The most fitting for Create operations. This code should signal backend-side resource creation and come along with a Location header that defines the most specific URL for that newly created resource.