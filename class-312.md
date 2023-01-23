# 312

## Status Codes Based On REST Methods

- In your own words, describe what each group of status code represents:  
**100’s =** Informational codes about information in the header  
**200’s =** Success codes  
**300’s =** Redirect codes so the client can reissue a request to the new location for the resource  
**400’s =** Client error codes for invalide requests sent by the client to the server  
**500’s =** Server error codes  

- What is a status code 202?  
Often used for async processing to let the client know the request was valid, but will finish in the future

- What is a status code 308?  
Permanent redirect to let the client know that the new URL should be used in future attempts to access this resource

- What code would you use if an update didn’t return data to a client?  
204

- What code would you use if a resource used to exist but no longer does?  
410

- What is the ‘Forbidden’ status code?  
403

## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

- Why do we need to pull our MongoDB database string out of our server and put it into our .env?  
This allows our backend to connect to our database.

- What is middleware?  
Functionality that executes after receiving the request, and before returning the response

- What does app.use(express.json()) do?  
Allows our express server to parse incoming requests with JSON payloads

- What does the /:id mean in a route?  
It's a parameter that can be accessed through the req.params object

- What is the difference between PUT and PATCH?  
PUT requires a full representation of the resource to be updated, PATCH requires only the specific pieces involved in the updated resource

- How do you make a default value in a schema?  
You make a default property that it will use if it's not passed in with the request

- What does a 500 error status code mean?  
Error on server

- What is the difference between a status 200 and a status 201?  
201 is for successfully creating an object, rather than the general success status of 200
