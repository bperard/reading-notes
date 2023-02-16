# 404

## nosql vs sql

- What type of database is the best fit for the complex query intensive environment?  
sql

- What type of database is the best fit for hierarchical data storage?  
nosql

- Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.  
SQL databases need more power for scaling (vertical), and NoSQL can scale by horizontally by expanding the infrastructure.

## sql modeling techniques

- Among data tables, what is a one-to-many relationship and how do we “relate” them?  
One item is related to many items (one author, multiple books), and they're related through a foreign key that's a reference to the primary key of the item.

- Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.  
create a diagram

- Explain the difference between a primary and foreign key.  
A primary is the unique identifier for an item in a table, a foreign key is used as a reference to the primary key of an item related in another table (author PK is the FK in the books table).

## sql vs nosql

- How do we treat keywords and parameters differently in SQL syntax?  
Keywords are uppercase, parameters are lowercase.

- Define normalization within the context of schemas and data.  
Normalization prepares data to be inserted into a table according to the rules of the database.

- Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.  
One to one is a unique relationship between two items (an id refers to a single item), one to many a unique item refers to many items (one refers to many items, but any item only has one price), many to many means items on both sides can refer to many items on the other side of the relationship (an order can have many items, and an item can be in many orders).
