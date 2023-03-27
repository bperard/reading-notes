# 434

## Review API Server Build

- Explain the different between a query string parameter and a path parameter.  
A query string is key value pair added at the end of the path following a question mark.  
*somesite.com/user?key=value*
A path parameter also a key value pair, but is part of the path, and the key is given defined in the route, and the value is typed into the path.  
*route: somesite.com/user/:id*
*path: somesite.com/user/3*

- What would our API URL with a path id parameter be given the following information:
Domain: http://our-site.com
v3
model name: stuff
id: things  
api/v3/stuff/:id

- We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.  
Rather than having to code the generic routes for all of our models, we can make an interface that allows these routes to dynamically be created for any model we want to have those routes, and then just provide that interface with the model.

## Review Auth Server Build

- Describe how you would use middleware to implement basic and bearer auth.  
Check for Basic Authentication Header, remove encoded user information, decode information, check db to verify information, return error or authentication information.

- Describe the handshake necessary to implement OAuth.  
User is sent to a third party for OAuth authentication, user provides their credentials to third party, third party uses your site info to know where to send the user after authentication, user arrives at landing page with credentials or error info, your site decides how to process credentials from the third party (add/update/verify credentials).

- Describe how Role Based Access Control works to a non-technical friend.  
A system has different defined roles created. These roles are assigned explicit access privileges that align with the given role. Accounts within this system are assigned with roles that determine their access. When access to resources is requested, an account role is checked to see if they have the required privileges.
