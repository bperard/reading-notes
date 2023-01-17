# 308

## API Design Best Practices

- What does REST stand for?  
Representational State Transfer

- REST APIs are designed around a ____.  
resource

- What is an identifier of a resource? Give an example.  
A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

```HTTP
https://adventure-works.com/orders/1
```

- What are the most common HTTP verbs?  
GET, POST, PUT, PATCH, and DELETE

- What should the URIs be based on?  
When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

- Give an example of a good URI.  

```HTTP
https://adventure-works.com/orders
```

- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?  
Try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request.

- What status code does a successful GET request return?  
200

- What status code does an unsuccessful GET request return?  
404

- What status code does a successful POST request return?  
201

- What status code does a successful DELETE request return?  
204
