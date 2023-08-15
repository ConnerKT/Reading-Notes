# Navigation Properties and Routing

This topic is important to me because I want to have code that is reusable and more organized.

## [Retrospective 14](https://connerkt.github.io/Reading-Notes/401/Class14/Retro14)

## References

[Routing within MVC](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/controllers-and-routing/asp-net-mvc-routing-overview-cs)

[Routing within Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/routing?view=aspnetcore-3.1)

## Routing within MVC

**Routing** in an MVC (Model-View-Controller) application refers to the process of determining how incoming URLs should be mapped to controllers and actions in order to handle user requests. It's a crucial mechanism that allows the application to understand which controller and action should be invoked based on the URL provided by the user.

Routing in MVC serves as a bridge between the user's request and the appropriate code that should handle that request.

This is how it works:
URL Parsing, Route Configuration, Route Matching, Controller and Action Selection, Parameter Binding, Action Execution.

Routing provides a way to create clean and user-friendly URLs for different parts of an application, making the application's structure more intuitive for both users and developers. It allows for the separation of concerns, where the routing logic handles the URL-to-action mapping, and the controllers handle the specific business logic for each action.

## Routing in ASP.NET Core

### Overview

Routing in ASP.NET Core follows the same fundamental principles as ASP.NET MVC, but with some differences due to the modular and flexible nature of the ASP.NET Core framework.

### Key Concepts

- **Routing:** The process of mapping incoming URLs to actions in controllers.

### Routing in ASP.NET Core

- ASP.NET Core uses the `Routing` middleware to handle URL routing.

- The routing configuration is often defined in the `Startup` class.

- ASP.NET Core supports attribute-based routing and convention-based routing.

### Attribute-Based Routing

- Controllers and actions can use attributes to define the route patterns.

- The `[Route]` attribute specifies the URL template for an action.

### Convention-Based Routing

- Convention-based routing is configured using the `UseEndpoints` method in `Startup.Configure`.

- Routes are defined based on conventions, such as `{controller}/{action}/{id}`.

### Route Templates

- Route templates are used to define dynamic parts of URLs and route parameters.

- Route parameters are enclosed in curly braces, like `{controller}` or `{id:int}`.

### Route Constraints

- Constraints can be added to route parameters to restrict the values they can accept.

- Constraints can be specified using predefined constraints or custom regular expressions.

### Areas and Routes

- ASP.NET Core supports areas, which allow for segmenting large applications into smaller modules.

- Areas can have their own route configuration, allowing for separate routing rules.

### URL Generation

- The `IUrlHelper` interface provides methods to generate URLs based on route names or route data.

### Benefits

- Routing enables clean and structured URLs in ASP.NET Core applications.

- Attribute-based and convention-based routing offer flexibility in defining routes.

- Centralized routing configuration simplifies URL handling.

### Practical Use Cases

- Mapping URLs to various parts of an application, including controllers and actions.

- Creating user-friendly and SEO-friendly URLs.

### Conclusion

Routing is a fundamental aspect of ASP.NET Core that enables the mapping of URLs to actions in controllers. Whether using attribute-based or convention-based routing, understanding how routing works is crucial for building organized and user-friendly web applications.

## Things I want to know more about

I want to learn how to build my own API's using the best techniques.

I want to learn the importance of routing within MVC and Core, and the differences.