# Identity

This topic is important to me because I want to be able to create an experience in my web applications that apply authentication.

## [Retrospective 18](https://connerkt.github.io/Reading-Notes/401/Class18/Retro18)

## References

[Intro to Identity](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.1&tabs=visual-studio%2Caspnetcore2x)

[Identity Demystified](https://freetimeprogrammer.com/blog/1-aspnetcore-auth-system-demystified/)

## Intro to Identity Notes

Its an API that supports UI login functionality

Manages users,passwords, profile data, roles, claims, tokens, email confirmation, and more!

Its configured using a SQL server DB to store all the data.

This is how we add authentication!

[Step by Step](https://www.c-sharpcorner.com/article/using-identity-in-asp-net-core-mvc-authentication/)

1. Add Identity to Your Project
    - Install the Microsoft.AspNetCore.Identity NuGet package in your ASP.NET Core project.

2. Configure Identity in Startup.cs
    - In the ConfigureServices method, configure Identity services, including user and role settings.

3. Database Setup
    - Identity data is stored in a database. Configure a database context and migrations to create the necessary tables.

4. User Registration and Login
    - Use the Identity APIs to handle user registration and authentication.

5. Authorization
    - Implement role-based or claims-based authorization using the [Authorize] attribute.

## Identity Demystified

[Source](https://freetimeprogrammer.com/blog/1-aspnetcore-auth-system-demystified/)

This site breaks down whats going on in the breakdown for Identity.

- Understanding authentication vs. authorization.
- Authentication schemes and handlers.
- Various authentication methods: cookies, JWT, OAuth.
- Policy-based authorization.

- ASP.NET Core uses authentication middleware to handle authentication and authorization.
- The blog explains how to add authentication middleware to the pipeline.

## Things I want to know more about

I want to understand how complicated this is to add to my own projects, I want to be good at doing it.

I want to learn more about the different libraries that can do authentication, if there is any.
