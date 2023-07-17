# Object Oriented Principles Notes

This topic is important to me because I want to learn about structuring my code for OOP and becoming a better, more efficient programmer.

## [Retrospective 6](https://connerkt.github.io/Reading-Notes/401/Class06/Retro06)

## References

[Inheritance](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/inheritance)
[Abstract](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members)
[Polymorphism](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/polymorphism)
[OOP Principes](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/object-oriented-programming)

## Inheritance

One of the three primary characteristics of OOP.

**Inheritance** enables you to create new classes that reuse, extend, and modify the behavior defined in other classes.

The class that is inherited from is called the base class. The members that inherit are called derived classes.

A derived class can have only one direct base class.

But each derived class represents different specializations of the base class.

Ex.

        Animal Class is the base class, and it has two derived classes, Mammal and Reptile.

    public class Vehicle
    {
        public string Brand { get; set; }
        public int Year { get; set; }

        public void Start()
        {
            Console.WriteLine("Engine started!");
        }

        public void Stop()
        {
            Console.WriteLine("Engine stopped!");
        }
    }
So if you make a class from this vehicle, it will inherit the methods, so we can reuse them, or modify them for this derived class.

    public class Car : Vehicle
    {
        public void Accelerate()
        {
            Console.WriteLine("Car accelerating!");
        }
    }

## Abstract

The **Abstract** keyword enables you to create classes and class members that are incomplete and must be implemented in a derived class.

**Sealed** enables you to prevent the inheritance of a class or certain class members.

Ex.
    public abstract class A
    {
        // Class members here.
    }

Abstract classes and members are useful when you want to define a common base with certain shared behaviors but leave the specific implementation details to derived classes. By marking a class or member as abstract, you ensure that it can only be used in a subclass or must be overridden, promoting a more flexible and extensible code structure.

## Polymorphism

**Polymorphism** is often referred as the third pillar of OOP, after encapsulation and inheritance.

The ability of an object to take on many forms. 

**Polymorphism** is a powerful concept that enables code to be more extensible, maintainable, and adaptable to different scenarios. It allows you to write code that can handle multiple types of objects in a uniform way, enhancing code reusability and promoting a more modular design.

## OOP Principles

The four basic principles of OOP is:

1. Abstraction
2. Encapsulation
3. Inheritance
4. Polymorphism

These principles collectively form the foundation of OOP and guide the development of software systems. By following these principles, you can create code that is more modular, maintainable, extensible, and reusable. OOP allows you to model real-world entities as objects, encapsulate their data and behavior, establish relationships between objects through inheritance and composition, and leverage polymorphism to write code that works with objects in a uniform and flexible manner.

## Things i want to know more about

I want to know the best process to go through in order to create programs that are Object Orientated.

I want to know how to practice a mindset so I make it an habit to make projects OOP.


