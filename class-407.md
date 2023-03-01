# 407

## Intro to JWT

- What is a JSON Web Token (JWT)?  
A JSON Web Token (JWT) is a compact, URL-safe means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using cryptography to ensure that the claims are not tampered with during transmission.

- When should we use JSON Web Tokens?  
JWTs are often used as a means of authentication and authorization in web applications and APIs.

- Claims are expected in which structural component of a JWT?  
Claims are expected in the payload component of a JWT.

## Are JWTs Secure?

- If I get a JWT and I can decode the payload, how can we call that secure?  
The claims in a JWT are base64-encoded and can be easily decoded to retrieve the original JSON object. It is important to note that the claims are not encrypted, so they can be read by anyone who has access to the token. For this reason, sensitive information should not be included in the JWT claims, and the token should be transmitted over a secure channel to prevent eavesdropping and tampering. However, without the proper key the payload can't be changed without showing the token has been tampered with.

- If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.  
If sending a JWT, both the sender and the receiver must know the secret key that is used to sign the token. The secret key is a shared secret between the parties that is used to create and verify the signature of the JWT.

- Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.  
Concatenated content and secret can be sent and received securely by using a shared secret key and a secure communication channel.

## JWTs Explained

- Why use JWT?  
It allows parties to share information in a way that's easy to show whether or not an outside party has tampered with the payload.

- JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.  
JWTs are easy to use, small, and tamper-proof which makes them an ideal mechanism for sharing information that isn't highly sensitive, but does require proof that an outside party hasn't altered it (authentication).

- What are the three components (the structure) of a JWT signature?  
A JWT typically consists of three parts separated by dots: the header, the payload, and the signature. The header specifies the type of token and the cryptographic algorithm used to sign the token, while the payload contains the claims or information about the user that the token represents. The signature is a hash of the header and payload, signed using a secret key that is shared between the two parties.
