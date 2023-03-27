# 433

## What is Role Based Access Control (RBAC)?

- What is Role Based Access Control (RBAC)?  
Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

- Share some an example of RBAC including all possible CRUD operations and correlating roles.  
A manager can create & delete employees, an employee can create/update/delete their work files, a client can read their reports. An admin is unrestricted and can turn everything to crud if oppose them.

- What are the Benefits of RBAC?  
Reducing admin work & IT support, maximizing operational efficiency, and improving compliance.

## react-cookie library & react-cookies component

- Describe some react-cookie features.  
<CookiesProvider /> Set the user cookies  
useCookies(*[dependencies]*) Access and modify cookies using React hooks.  
setCookie(*name, value, [options]*) Set a cookie value  
removeCookie(*name, [options*]) Remove a cookie  
withCookies(Component) Give access to your cookies anywhere.  

- Describe some react-cookies features.  
.load(*name, [doNotParse]*) Load the cookie value.  
.loadAll() Load all available cookies.  
.select(*[regex]*) Find all the cookies with a name that match the regex.  
.save(*name, value, [options]*) Set a cookie.  
.remove(*name, [options]*) Remove a cookie.  

- Which library would you prefer? Why?  
React cookie because the last publish was 2 years ago (rather than four), and it was ~433k weekly downloads (rather than 33k).
