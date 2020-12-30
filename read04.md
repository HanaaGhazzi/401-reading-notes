# Advanced Mongo/Mongoose


## Why would a developer choose to make data models?
_Faster performance,Clearer scope_

## What purpose do CRUD operations serve?
 
 CREATE/READ/UPDATE/DELETE

## What kind of database is Postgres? What kind of database is MongoDB?
PostgreSQL relational database management system
MongoDB NoSQL database program
## What is Mongoose and why do we need it?
Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment

## Describe how NoSQL Databases scale horizontally
by adding more machines

## Give one strong argument for and against NoSQL Databases
for: Flexible Scalability against: Less Support

## Name 3 cloud based NoSQL Databases
mLab/DynamoDB/Amazon Web Services

## Terms

- database: A database is an organized collection of data, generally stored and accessed electronically from a computer system
- data model: constructors that take a schema and create an instance of a it to be stored in db.
- CRUD: mainly: create, read, update and delete.
- schema: shape of the document that is enforced via the application layer.
- sanitize: computer data to be checked by software to see if it contains any harmful data.
- Structured Query Language (SQL): mainly to access and manipulate databases
- Non SQL (NoSQL): database to accommodate a wide variety of data models,without using SQL
- MongoDB: mainly it is a database used for high volume data storage.
- Mongoose: provides an interface to the database for creating, querying, updating, deleting records..
- record: Records are composed of fields, each of which contains one item of information.
- document: equivalent to records or rows of data in SQL.
- Object Relation Mapping (ORM): to write queries using the object-oriented paradigm of your programming language.

## Repository Design Pattern 

> "A Repository mediates between the domain and data mapping layers, acting like an in-memory domain object collection. Client objects construct query specifications declaratively and submit them to Repository for satisfaction. Objects can be added to and removed from the Repository, as they can from a simple collection of objects, and the mapping code encapsulated by the Repository will carry out the appropriate operations behind the scenes."


**The separation of data access from business logic have many benefits. Some of them are:**

1. Centralization of the data access logic makes code easier to maintain
2. Business and data access logic can be tested separately
3. Reduces duplication of code
4. A lower chance for making programming errors


## Testing Node.js + Mongoose with an in-memory database

### In-memory database pros & cons


#### Pros:

- No need for mocks: Your code is directly executed using the in-memory database, exactly the same as using your regular database.
- Faster development: Given that I don't need to build a mock for every operation and outcome but only test the query, I found the development process to be faster and more straightforward.
- More reliable tests: You're testing the actual code that will be executed on production, instead of some mock that might be incorrect, incomplete or outdated.
- Tests are easier to build: I'm not an expert in unit testing and the fact that I only need to seed the database and execute the code that I need to test made the whole process a lot easier to me.

#### Cons:

- The in-memory database probably needs seeding
- More memory usage (dah)
- Tests take longer to run (depending on your hardware).

