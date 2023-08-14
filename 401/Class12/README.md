# Entity Framework and APIs

This topic is important to me because I want to learn how to create my own Apis

## [Retrospective 12](https://connerkt.github.io/Reading-Notes/401/Class12/Retro12)

## References

[MVC with EF](https://docs.microsoft.com/en-us/aspnet/core/data/ef-mvc/intro)

[Entity Framework Core](https://docs.microsoft.com/en-us/ef/core/)

[Data Seeding](https://docs.microsoft.com/en-us/ef/core/modeling/data-seeding)

[Entity Framework Core](https://docs.microsoft.com/en-us/aspnet/core/data/ef-rp/intro?view=aspnetcore-2.1&tabs=visual-studio)

[User Secrets](https://codefellows.github.io/code-401-dotnet-guide/resources/user-secrets.html)

[Intro to APIs](https://youtu.be/aIkpVzqLuhA)

# Introduction to Entity Framework in ASP.NET Core MVC

This tutorial introduces Entity Framework (EF) in the context of ASP.NET Core MVC. Entity Framework is an object-relational mapper that simplifies database operations by allowing developers to work with databases using C# or VB.NET code, instead of writing SQL queries.

- **ORM (Object-Relational Mapping):** Entity Framework is an ORM tool that bridges the gap between object-oriented programming and relational databases. It allows you to work with database objects as if they were regular C# objects.

- **DbContext:** DbContext is the main class that provides an interface to interact with the database. It represents the session with the database, allowing you to query and manipulate data.

- **Entities:** Entities are C# classes that represent tables in the database. Each instance of an entity represents a row in the table.

- **LINQ (Language Integrated Query):** Entity Framework uses LINQ to query and manipulate data. LINQ provides a more readable and type-safe way to work with data compared to writing raw SQL queries.

## Steps Covered

1. **Create a Model:**
   - Define C# classes to represent your database tables (entities).

2. **Create a DbContext:**
   - Create a subclass of DbContext to establish a connection to the database and provide an interface to interact with it.

3. **Configure Entities:**
   - Use data annotations or fluent API to configure relationships, data types, and other attributes of your entities.

4. **Querying Data:**
   - Use LINQ to query data from the database using the DbContext.

5. **Updating Data:**
   - Add, modify, and delete data using methods provided by the DbContext.

6. **Database Migrations:**
   - Use migrations to manage changes to the database schema over time.

## Benefits

- **Code-Centric Approach:** Developers can work with databases using familiar programming concepts, making it easier to manage and maintain data-related code.

- **Type Safety:** Entity Framework provides type-safe queries and operations, reducing the likelihood of runtime errors.

- **Cross-Platform:** Entity Framework works with various database providers, allowing your ASP.NET Core applications to run on different platforms and use different databases.

- **Automatic SQL Generation:** Entity Framework generates SQL queries based on your LINQ queries, reducing the need for writing raw SQL.

## Practical Use Cases

- **Web Applications:** Building web applications that need to interact with a database to store and retrieve data.

- **Enterprise Applications:** Developing enterprise-level applications with complex data models and relationships.

- **APIs:** Creating APIs that handle data storage and retrieval for various client applications.

## Things I want to know more about

I want to learn more about the databse relationships.

I want to learn more about framework migrations.


