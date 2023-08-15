# Dependency Injection & Repository Design Pattern

This topic is important to me because I want to have code that is reusable and more organized.

## [Retrospective 13](https://connerkt.github.io/Reading-Notes/401/Class13/Retro13)

## References

[Dependency Injection](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection)

[Repository Pattern](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/repository-pattern?view=aspnetcore-2.1)

[Repository Design Pattern](https://medium.com/@pererikbergman/repository-design-pattern-e28c0f3e4a30)

[SOLID Principles](https://www.telerik.com/blogs/30-days-of-tdd-day-five-make-your-code-solid)

[Why SOLID Matters](https://www.telerik.com/blogs/why-solid-matters)

[SOLID Principles in Pictures](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898)

## Notes

Dependency Injection is a software design pattern used to manage dependencies between components in a more flexible and maintainable way. It involves providing external dependencies to a class rather than letting the class create them internally.

## Key Concepts

- **Dependency:** A service or object that another class depends on to perform its tasks.

- **Dependency Injection Container:** A container or framework that manages the creation and lifetime of dependencies. It resolves and injects dependencies into classes that require them.

- **Injection:** The process of passing dependencies to a class from the outside, usually through constructor parameters or setters.

## Benefits

1. **Decoupling:** Components are decoupled from their dependencies, making the codebase more modular and adaptable to change.

2. **Testability:** DI makes it easier to test components in isolation by injecting mock or test implementations of dependencies.

3. **Flexibility:** You can easily swap or change dependencies without modifying the dependent classes.

4. **Readability:** Dependencies are explicitly declared, enhancing code readability and understanding.

5. **Maintainability:** Changes to dependencies impact only the registration code, reducing the ripple effect of changes.

6. **Inversion of Control (IoC):** DI is a key part of IoC, where control over object creation is inverted to a central container.

## How to Implement DI

1. **Identify Dependencies:** Determine which classes require dependencies to function properly.

2. **Create Interfaces:** Define interfaces for dependencies to enable loose coupling.

3. **Configure Container:** Set up a DI container or framework (e.g., ASP.NET Core's built-in container) to manage dependencies.

4. **Register Dependencies:** In the container's configuration, register interfaces with their corresponding implementations.

5. **Inject Dependencies:** In classes requiring dependencies, use constructor injection or property injection to receive the dependencies.

## Types of Injection

1. **Constructor Injection:** Dependencies are passed through the constructor when creating an instance of the dependent class.

2. **Property Injection:** Dependencies are set as properties of the dependent class after its creation.

3. **Method Injection:** Dependencies are provided as parameters to methods where they are needed.

## Best Practices

1. **Use Interfaces:** Depend on interfaces rather than concrete implementations to allow for flexibility and easy mocking.

2. **Limit Container Usage:** Only use the DI container at the composition root to maintain clear control over dependencies.

3. **Keep Dependencies Simple:** Dependencies should do one thing well and have a clear purpose.

Dependency Injection is a powerful pattern that improves code quality, testability, and maintainability. It encourages loose coupling and allows for better control over dependencies in complex applications.

## Key Concepts

- **SOLID Principles:** SOLID is an acronym that stands for Single Responsibility Principle (SRP), Open-Closed Principle (OCP), Liskov Substitution Principle (LSP), Interface Segregation Principle (ISP), and Dependency Inversion Principle (DIP).

## SOLID Principles

1. **Single Responsibility Principle (SRP):**
   - A class should have only one reason to change.
   - A class should have one primary responsibility.
   
2. **Open-Closed Principle (OCP):**
   - Software entities should be open for extension but closed for modification.
   - New features can be added without altering existing code.

3. **Liskov Substitution Principle (LSP):**
   - Subtypes must be substitutable for their base types without affecting program correctness.
   - Inheritance should not break behavior or contracts.

4. **Interface Segregation Principle (ISP):**
   - Clients should not be forced to depend on interfaces they do not use.
   - Smaller, more specific interfaces are preferable to larger, general ones.

5. **Dependency Inversion Principle (DIP):**
   - High-level modules should not depend on low-level modules. Both should depend on abstractions.
   - Abstractions should not depend on details. Details should depend on abstractions.

## Applying SOLID Principles

1. **Identify Responsibilities:** Break down classes into single responsibilities.

2. **Abstraction and Encapsulation:** Use interfaces and abstract classes to define contracts and hide implementation details.

3. **Inheritance and Polymorphism:** Ensure that derived classes can be substituted for base classes without altering program behavior.

4. **Dependency Injection:** Design classes so that they depend on abstractions rather than concrete implementations.

## Benefits

- **Code Maintainability:** SOLID principles lead to code that's easier to understand, extend, and modify.

- **Flexibility:** Code adhering to SOLID principles can adapt to changing requirements and new features.

- **Testability:** SOLID code is more testable, as classes can be isolated and dependencies injected.

## Practical Use Cases

- **Large Codebases:** Applying SOLID principles helps manage complexity and maintain large projects.

- **Collaborative Development:** SOLID principles facilitate collaboration among developers by promoting clean and modular code.

## Conclusion

SOLID principles provide a guideline for designing well-structured, maintainable, and flexible code. By adhering to these principles, developers can create software that's easier to maintain, extend, and test.

## Things I want to know more about

I want to learn more about using Dependency Injection, and why I would use it for my projects.

I want to learn more about practicing SOLID principles so I can be a more proficient programmer.
