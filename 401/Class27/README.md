# MVC Forms

This topic is important to me because I'm interested in how to make web applications with razor pages and see the difference between react sites.

## [Retrospective 27](https://connerkt.github.io/Reading-Notes/401/Class16/Retro27)

## References

[View Models](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/overview?view=aspnetcore-2.2)

[4 Ways to make a form in .NET MVC](https://www.completecsharptutorial.com/asp-net-mvc5/4-ways-to-create-form-in-asp-net-mvc.php)

## View Models

The view handles the app's data presentation and UI. A view is an HTML template with embedded Razor markup. Razor markup is code that interacts with HTML markup to produce a webpage that's sent to the client.

Views help serperation of concerns within an MVC application by seperating the UI markup from other parts of the app. 

## 4 Ways to make a form in .NET MVC

1. **Using HTML Form**:
   - The simplest method involves using standard HTML forms in MVC views.
   - HTML `<form>` elements are used to define the form and its elements (input fields, buttons, etc.).
   - The form can be submitted to a controller action for further processing.

2. **Using Html.BeginForm()**:
   - `Html.BeginForm()` is a helper method that generates the opening `<form>` tag with the correct action and method attributes.
   - This method simplifies form creation and ensures that the form is properly associated with a controller action.

3. **Using Ajax.BeginForm()**:
   - `Ajax.BeginForm()` is a helper method that creates an AJAX form, allowing asynchronous form submission without a full page refresh.
   - It utilizes JavaScript to handle the asynchronous behavior and update specific parts of the page based on the AJAX response.

4. **Using Form Tag Helper**:
   - Form Tag Helper (`<form asp-controller="" asp-action="">`) is a newer and more intuitive way to create forms in ASP.NET Core.
   - It uses tag helpers in Razor views to simplify form creation, making the code cleaner and more readable.
   - The `asp-controller` and `asp-action` attributes specify the controller and action to which the form will be submitted.

## Things I want to know more about

I want to know more about are using Razor pages to make web sites.
I want to know more about why people are using Razor pages.