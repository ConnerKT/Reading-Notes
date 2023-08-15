# Testing and Swagger and Deployment

This topic is important to me because I want to be able to have a series of test that I can run to ensure my application runs.

## [Retrospective 17](https://connerkt.github.io/Reading-Notes/401/Class17/Retro17)

## References

[Swagger](https://docs.microsoft.com/en-us/aspnet/core/tutorials/web-api-help-pages-using-swagger?tabs=visual-studio&view=aspnetcore-2.1)

[Unit Testing](https://docs.microsoft.com/en-us/aspnet/mvc/overview/older-versions-1/unit-testing/creating-unit-tests-for-asp-net-mvc-applications-cs)

[Testing Controllers](https://docs.microsoft.com/en-us/aspnet/core/mvc/controllers/testing?view=aspnetcore-2.1)

## Swagger Notes

- Swagger helps generate interactive API documentation for ASP.NET Core Web API projects.
- Developers can use Swagger UI to explore and test API endpoints.

### Steps

1. **Create a new ASP.NET Core Web API project**
   - Use Visual Studio or the command-line interface to create a new ASP.NET Core Web API project.

2. **Install Swashbuckle NuGet package**
   - Open the project in Visual Studio.
   - Install the `Swashbuckle.AspNetCore` NuGet package.

3. **Configure Swagger services**
   - In the `Startup.cs` file, add services for Swagger in the `ConfigureServices` method.
   - Use the `services.AddSwaggerGen` method to configure Swagger options and document generation settings.

4. **Configure Swagger UI**
   - In the `Startup.cs` file, add middleware for Swagger in the `Configure` method.
   - Use the `app.UseSwagger` and `app.UseSwaggerUI` methods to configure the Swagger UI endpoint and UI settings.

5. **Customize Swagger documentation**
   - Add XML comments to your API controllers and models.
   - Configure Swagger to include XML comments for generating accurate API documentation.

6. **Test the Swagger UI**
   - Run the project.
   - Access the Swagger UI at `/swagger`.

## Unit Testing Notes

We want to write unit test for our controllers in our web applications.

You can test the view returned by a controller action, how to test the View Data returned by a controller action, and how to test whether or not one controller action redirects you to a second controller action.

Write Unit Tests

1. Create a new class for your controller's unit tests (e.g., HomeControllerTests).
2. In your test class, you'll need to set up the following:
        A reference to the controller being tested.
        Mocked instances of services or dependencies that your controller depends on.

3. Define Test Cases

    Define individual test methods within your test class.
    Each test method should focus on testing a specific scenario or functionality of your controller action.

## Testing Controllers

**Unit Test** involve testing a part of an app in isolation from its infrastructure and dependencies.

    Write test methods to test your controller actions.
    Use the test client to send HTTP requests and receive responses.
    Assert the responses, status codes, view results, or data returned by the actions.

    Unit testing ASP.NET Core MVC controllers helps ensure the correctness of your application's behavior.
    xUnit and Moq are powerful tools for creating effective and reliable controller tests.

## Things I want to know more about

I want to learn when I'll use unit testing in a work place setting.

I want to learn the different libraries that I can use to build things cool, like with Swagger for example.