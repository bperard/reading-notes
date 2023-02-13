# 402

## An introduction to NodeJS and Express

- Explain middleware, answer as though I were a non-technical recruiter.  
When a request is made to a server, the middleware is the code that is executed after receiving a request, and before returning the response.

- Express the most popular __ __ ____.  
Node web framework

- Express is “unopinionated.” What does that mean?  
It is up to the developer to decide how to handle tasks within the framework, rather than having a methodology imposed by the framework.

- What is a module and why is modularity useful to us as developers?  
A module is a JS library or file that you can import into other code using Node's require function. Modules allow code to be organized into more manageable pieces, which makes our code easier to maintain.

## What is NPM?

- What version of npm are you running on your machine?  
9.4.0

- What command would you type to install a library/package called ‘jshint’ into your node project?  
npm install jshint

## What is TDD?

- Explain why tests are important. Please explain as though I were your non technical elder.  
Tests allow us to independently verify the functionality of a piece of our code, which is helpfuly to confirming changes made elsewhere, or within, do not affect the output.

- What are three expected benefits of testing  
Significant reductions in defect rates, reduction in effort in project final stages, and improved design qulaities.

- Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.  
Poor maintenance of the test suite, and abandoned (or seldom run) test suite.

## CI/CD

- What are three benefits of Continuous Integration?  
 Ensures everyone's changes integrate which helps catch bugs and reduce merge conflicts.

- What is the difference between Continuos Delivery and Continuous Deployment?  
Continuous delivery is a development process that allows for release at any time, and continuous deployment is a further extension of that which allows new features to be released immediately without any major downtime.

- Explain how GitHub fits into this process assuming the listener comes from a non-technical background  
GitHub allows code to maintained in a common repository, keeping all of the changes and updates in one place. As new code needs to be integrated into production, tests are run to verify it is ready for deployment. This continuous integration process allows new features to be continuously deployed in conjunction with their development.
