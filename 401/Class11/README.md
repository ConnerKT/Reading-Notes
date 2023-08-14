# Introduction to Databases and ERDs

This topic is important to me because I want to form databases for my application to hold data and be able to learn how to set relations.

## [Retrospective 11](https://connerkt.github.io/Reading-Notes/401/Class11/Retro11)

## References

[Data Models](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/complex-data-model?view=aspnetcore-2.0)

[DBMS](https://www.tutorialspoint.com/dbms/dbms_overview.htm)

## Data Models

- **Complex Data Model:** Developing a more intricate data model using Entity Framework Core, including multiple entities with relationships.
  
- **Relationships:** Creating associations between entities, such as one-to-many and many-to-many relationships.
  
- **Navigation Properties:** Defining navigation properties in entities to navigate between related data.

- **DbContext:** Creating a `DbContext` class to represent the database context and manage interactions with the database.

## Steps Covered

1. **Creating the Model:**
   - Defining multiple entity classes with properties representing different aspects of the data.

2. **Defining Relationships:**
   - Establishing relationships between entities using navigation properties (e.g., one-to-many, many-to-many).

3. **Creating DbContext:**
   - Creating a `DbContext` class that inherits from `DbContext` to represent the database context and manage interactions with the database.

4. **Seed Data:**
   - Adding sample data to the database context to facilitate testing and demonstration.

5. **Using DbContext in a Controller:**
   - Injecting the database context into a controller to access and manipulate data.

6. **Displaying Related Data:**
   - Utilizing navigation properties to display related data in views, enhancing the user experience.

## Benefits

- **Data Complexity Handling:** Learn how to manage and represent complex data scenarios in an organized and efficient manner.

- **Navigation:** Understand how navigation properties simplify data retrieval and presentation, particularly when dealing with related data.

- **ASP.NET Core MVC Integration:** Integrate the complex data model seamlessly into an ASP.NET Core MVC application.

- **Entity Framework Core:** Gain experience using Entity Framework Core to handle database interactions and queries.

## Data Models Questions

1. Do some research on what a Database Schema is.
        What is a Schema?
        Why do we use them?
        What do they look like?
2. What are the different types of Database Keys?
        What is a Primary Key?
        What is a Foreign Key?
        What is a Composite Key?
        How are they different? When do you use 1 over the others?

## Data Models Answers

1. A schema is essentially the blueprint.
    We use it to define how the data is going to be structured.
    They usually are set with how the data is going to be for the end user.
2. The colum or columns that contain values that uniquely identify each row in a    table.
    A column used to link data between tables.
    A combination of two or more columns in a table to uniquely identify each row.
    Primary when you need a unique identifier.
    Foreign when you want to establish relationships between tables
    Composite when a single column isn't enough for uniqueness.

## DBMS

A **DBMS** stores data in such a way that it becomes easier to retrieve, manipulate, and produce information.

A modern DBMS has the following:

- Real-world Entity

- Relation-based tables

- Isolation of data and application

- Less redundancy

- Consistency

- Query Language

- ACID Properties

- Multiuser and Concurrent Access

- Multiple views

- Security

A typical DBMS has **users** with different rights and permissions who use it for different purposes.

Some users retrieve data and some back it up.

The roles can be categorized as:

- Admins

- Designers

- End Users

## DBMS Questions

1. What are Relationships in a relational database?

    What is a 1:1 relationship?
    What is a Many:Many relationship?
    How about a 1: Many or a Many:1?

## DBMS Answers

1. 

- A connection between two tables where each record in the first table is related to exactly one record in the second table.
- When records in one table can be associated with multiple records in another table.
- Where records in one table can be related to multiple records in another table, but records in the second table are related to only one record in the first table.

## Things I want to know more about

I want to know more about setting the relationships between tables.

I want to learn how to get better with understanding when I need to connect different tables.

