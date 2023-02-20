# 406

## Securing Passwords

- Explain to a non-technical friend how you would safely hash and store a password.  
Hash passwords so they're not saved as plain-text in your database, and keep access to authentication endpoints internal in your API structure.

- What is Bcrypt?  
Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

- Why might you use something like Bcrypt?  
To make brute force attacks slower and minimize the impact.

## Basic Auth

- What is Basic Authentication?  


- What properties are necessary in the header of a Basic Auth request?  
In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic < credentials >, where credentials is the Base64 encoding of ID and password joined by a single colon :.

- How are username:password in Basic Auth encoded?  
They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

## OWASP auth cheatsheet

- Define the authentication process to a non-technical recruiter.  
A user identifies themself in the authentication process by providing a piece of private information that links them to a specific identity to be used in a system. After that, a management system is used to maintain this identity within the system for a session (or possibly longer/shorter depending on design) so that this authentication persists during subsequent requests.

- How should your error messaging respond (both HTTP and HTML)? Why?  
Respond with a generic message so that an attacker can use the response to gain further information about the credentials provided during the attack.

- Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.  
[OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)
