# 315

## What is OAuth

- **What is OAuth?**  
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

- **Give an example of what using OAuth would look like.**  
Signing into a site using your Gmail account.

- **How does OAuth work? What are the steps that it takes to authenticate the user?**  
A site gves you a login option through another service, you're sent to sign in, and then the originating service is sent some of those credentials to use as your authentication.

- **What is OpenID?**  
In 2014, OpenID Connect was released, which reinvented OpenID as an authentication layer for OAuth.

## Authorization and Authentication flows

- **What is the difference between authorization and authentication?**  
Authentication identifies a user within a system, authorization determines user access to resources within that system.

- **What is Authorization Code Flow?**  
A user is authenticated, when a resource requires authorization the authenticated identity is passed off, the level of authorization is checked against what's required for the requested resource, and the user is either given the resource or told they aren't authorized.

- **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**  

1. The user clicks Login within the application.

2. Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

3. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) along with the code_challenge.

4. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

5. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

6. Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

7. Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (/oauth/tokenendpoint).

8. Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

9. Your Auth0 Authorization Server responds with an ID token and access token (and optionally, a refresh token).

10. Your application can use the access token to call an API to access information about the user.

11. The API responds with requested data.

- **What is Implicit Flow with Form Post?**  

1. The user clicks Login in the app.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

5. Your Auth0 Authorization Server redirects the user back to the app with an ID Token.

- **What is Client Credentials Flow?**  

1. The application authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (/oauth/token endpoint).

2. Auth0 Authorization Server validates the Client ID and Client Secret.

3. Auth0 Authorization Server responds with an Access Token.

4. The application can use the access token to call an API on behalf of itself.

5. The API responds with requested data.

- **What is Device Authorization Flow?**  

1. The user starts the app on the device.

2. The device app requests authorization from the Auth0 Authorization Server using its Client ID (/oauth/device/code endpoint).

3. The Auth0 Authorization Server responds with a device_code, user_code, verification_uri, verification_uri_complete expires_in (lifetime in seconds for device_code and user_code), and polling interval.

4. The device app asks the user to activate using their computer or smartphone. The app may accomplish this by:

- asking the user to visit the verification_uri and enter the user_code after displaying these values on-screen

- asking the user to interact with either a QR Code or shortened URL with embedded user code generated from the verification_uri_complete

- directly navigating to the verification page with embedded user code using verification_uri_complete, if running natively on a browser-based device

5. The device app begins polling your Auth0 Authorization Server for an Access Token (/oauth/token endpoint) using the time period specified by interval and counting from receipt of the last polling request's response. The device app continues polling until either the user completes the browser flow path or the user code expires.

6. When the user successfully completes the browser flow path, your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token). The device app should now forget its device_code because it will expire.

7. Your device app can use the Access Token to call an API to access information about the user.

8. The API responds with requested data.

- **What is Resource Owner Password Flow?**  

1. The user clicks Login within the application and enters their credentials.

2. Your application forwards the user's credentials to your Auth0 Authorization Server (/oauth/token endpoint).

3. Your Auth0 Authorization Server validates the credentials.

4. Your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token).

5. Your application can use the Access Token to call an API to access information about the user.

6. The API responds with requested data.
