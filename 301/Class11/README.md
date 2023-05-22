# MongoDB and Mongoose Notes

Im interested in the topic because I want to learn on how to use databases.

## [Retrospective 11](https://connerkt.github.io/Reading-Notes/301/Class11/Retro11)

## References

[NoSQL vs SQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool).
[SQL VS NOSQL VIDEO](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y).
[Mongoose API](https://mongoosejs.com/docs/api.html#Model).
[React Router](https://reactrouter.com/web/api/BrowserRouter).

## NoSQL vs SQL Notes

**NoSQL**(Not Only SQL). It's a type of database system that is designed to handle large amounts of data and provide flexibility in storing and retrieving that data.

NoSQL allows you to store data in different formats unlike traditional databases (SQL).

In NoSQL you don't have to define a specific structure in advance.

NoSQL databases are good at scaling. It distributes data across multiple servers, making it easier to handle the increased load.

**SQL**(Structured Query Language). Its a type of database system that uses a structured approach to store and organize data. Data is organized into tables, which are like grids with rows and columns. Each table has a predefined structure, meaning you need to define the columns and their data types before storing data.

SQL databases are good for applications where you need to maintain strict data consistency and integrity. They ensure that your data follows specific rules, and any changes to the data are carefully controlled. 

SQL databases provide a standardized way to retrieve, insert, update, and delete data using the SQL language, which is widely supported and understood by developers.

In summary, **NoSQL** databases are flexible, scalable, and suitable for handling large amounts of rapidly changing data, while **SQL** databases have a structured approach, enforce data integrity, and are commonly used in applications where maintaining strict relationships and consistency is important.

### NoSQL vs SQL Questions

1. Fill in the chart below with five differences between SQL and NoSQL databases:
    SQL:
    NoSQL:
1. What kind of data is a good fit for an SQL database?
2. Give a real world example.
3. What kind of data is a good fit a NoSQL database?
4. Give a real world example.
5. Which type of database is best for hierarchical data storage?
6. Which type of database is best for scalability?


### NoSQL vs SQL Answers

1. SQL: More structured,Data integrity,consistent, complex queries, Powerful
    NoSQL: Flexible,  scalability, large amounts of data, easy structure.
1. E-commerce platforms.
2. Online stores need to store customer details, orders, inventory management.
3. Real time data such as analytics
4. News station, gaming applications
5. SQL
6. NoSQL

## SQL and noSQL Video Notes

SQL gives a way for us to not only select data from a database but also add data.

Ex. **SELECT** id,name,price **FROM** products
(The bold are SQL Syntax and the rest are data/parameters)

The Database Structure: Its a relational database that works in certain ways.

They follow a Schema which outlines the fields, and records for our database.

All records have to follow this Schema.

Ex. Id, Name, Price, Description.

Each record have to follow this.

Usually with a database, you have multiple tables, which share relations.

Ex. User table, products table, orders table

The orders table would connect the relations for our tables.

Relational Databases allow us to connect different tables and use data in each.

Different types of relations are:
One-To-One: One table to one table
One-To-Many: One table to many
Many-To-Many: Connects different tables from one center table.

### SQL and noSQL Questions

1. What does SQL stand for?
2. What is a relational database?
3. What type of structure does a relational database work with?
4. What is a ‘schema’?
5. What is a NoSQL database?
6. How does it work?
7. What is inside of a MongoDB database?
8. Which is more flexible - SQL or MongoDB? and why.
9. What is the disadvantage of a NoSQL database?

### SQL and noSQL Answers

1. Structured Query Language
2. A database that organizes data and has relationships between the items.
3. Tables and columns.
4. The logical structure of a database.
5. A database for unstructured changing daa.
6. It follows a system for storing data without enforcing a schema.
7. Data is stored as documents,which are similar to json like.
8. MongoDB since its NoSQL.
9. Data may not be immediately consistent.

## Thing I want to know more about

I want to understand the differences between NoSQL and SQL more detailed.

How do you use databases in a daily project.

How important is having a database for a personal project.