# Data Transfer Objects

This topic is important to me because I want to be able to understand how to protect the data the user is accessing.

## [Retrospective 16](https://connerkt.github.io/Reading-Notes/401/Class16/Retro16)

## References

[Data Transfer Objects](https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5)

[How to use DTOs](https://www.infoworld.com/article/3562271/how-to-use-data-transfer-objects-in-aspnet-core-31.html)

## Create Data Transfer Objects

Before using DTOs, our web APIs exposes the database entities to the client. The client receives the data that maps directly to your database tables. 

If you want to do the following you might need to use a DTO:

- Remove circular references (see previous section).
- Hide particular properties that clients are not supposed to view.
- Omit some properties in order to reduce payload size.
- Flatten object graphs that contain nested objects, to make them more convenient for clients.
- Avoid "over-posting" vulnerabilities. (See Model Validation for a discussion of over-posting.)
- Decouple your service layer from your database layer.

DTOs, or Data Transfer Objects, serve a specific purpose in software development, particularly in scenarios involving data exchange between different layers of an application or between different applications.

## How to use DTOs

The biggest advantage of using DTOs is decoupling clients from your internal data structures.

## Benefits of Using DTOs

- **Decoupling:** DTOs decouple clients from internal data structures, enhancing application architecture.
  
- **Abstraction:** DTOs abstract domain objects from the presentation layer, facilitating layer-specific changes.

- **Data Hiding:** DTOs enable data hiding by allowing you to return only requested data, enhancing privacy.

## Creating an ASP.NET Core 3.1 API Project

- Create an ASP.NET Core project using Visual Studio 2019.
- Select the "API" project template.
- Configure project settings and ensure features like Docker support and HTTPS are unchecked.

## Why Use Data Transfer Objects (DTOs)?

- Exposing internal data structures through models is a design flaw.
- DTOs decouple layers and ease API, MVC, and messaging pattern implementations.
- DTOs are useful for passing lightweight objects in bandwidth-constrained environments.

## Using DTOs for Abstraction and Data Hiding

- DTOs abstract domain objects from the presentation layer.
- Changing presentation or domain layers becomes easier without affecting the other.
- DTOs enable data hiding by returning only requested data.

## Creating a DTO Class

- Define a DTO class with selected properties to transport specific data.
- Use DTOs to return only required data from methods.

## Immutability of DTOs

- DTOs transport data between layers and might be serialized.
- Immutability is crucial for DTOs, ensuring data integrity.
- Implement immutability using ReadOnlyCollection, System.Collections.Immutable, or C# 9 record types.

## DTO Serialization Challenges

- Serializing DTOs with related entities may lead to serialization problems.
- Lazy loading or asynchronous loading helps manage serialization of complex object graphs.
- DTOs typically contain data without business logic.

## Conclusion

Using Data Transfer Objects (DTOs) in ASP.NET Core 3.1 applications provides benefits like decoupling, abstraction, and data hiding. DTOs enhance the maintainability and scalability of your application by facilitating controlled data exchange between layers.

## Things I want to know more about

I want to learn how to practice using DTOs in my application.

I want to learn if using DTOs is a commonly used practice in bigger fields.

