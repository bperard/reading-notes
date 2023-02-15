# 403

## Review: ES6 Classes

- Classes are a template for creating ____.  
objects

- Can a class declaration be hoisted?  
no

- How would you describe a constructor and contextual “this” to a non-technical friend?  
The constructor adds properties to your class, and this refers to the specific object you're interacting with.

## Using Express Routing

- Within Express, what does routing refer to?  
Routing refers to how an application’s endpoints (URIs) respond to client requests.

- What is the difference between a route path and a route method?  
Path refers to the URI associated with the request, and method refers to the HTTP method used for the request.

- When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?  
Next passes control to the next handler, make sure to have a handler for the response so the client request is not left hanging.

## Express Routing

- What is an Express Router?  
Router is like a mini-Express application.

- By what mean do we initialize express.Router() in an express server?  
Require express, and then set express.Router() to a variable so we can use it on our routes.

- What do we use route middleware for?  
Route middleware in Express is a way to do something before a request is processed.
