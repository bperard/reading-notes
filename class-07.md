# Object Oriented Programming

## Domain Modeling

**Explain why we need domain modeling.**
Domain modeling allows us to create a conceptual model in code for a specific problem.

## HTML Table Basics

**Why should tables not be used for page layouts?**
Layout tables reduce accessibility for visually impaired users, tables produce tag soup, and tables are not automatically responsive.

**List and describe 3 different semantic HTML elements used in an HTML table.**
thead, tfoot, tbody

## Introducing Constructors

**What is a constructor and what are some advantages to using it?**
A constructor is just a function called using the *new* keyword. When you call a constructor, it will:

- create a new object
- bind this to the new object, so you can refer to this in your constructor code
- run the code in the constructor
- return the new object

**How does the term this differ when used in an object literal versus when used in a constructor?**
A constructor using the same code to initialize different objects, so this allows you to refer to a specific instance from the same constructor. Object literals don't have multiple instances, so it's not as useful since there aren't different instances.

## Object Prototypes Using A Constructor

**Explain prototypes and inheritance via an analogy from your previous work experience.**
When you're in a role (prototype) you inherit the responsibilities (methods and properties) of that role, but you will also have responsibilities that are specific to you that others in your role don't share.
