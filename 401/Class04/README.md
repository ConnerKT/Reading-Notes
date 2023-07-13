# Classes and Memory Management Notes

This topic is important to me because I want to be able to be better at performing OOP actions in my code, and keeping my code object orientated.

## [Retrospective 4](https://connerkt.github.io/Reading-Notes/401/Class04/Retro04)

## References

[Classes](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/classes)

[Constructors](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/constructors)

[Properties](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/properties)

[Stack and Heap](https://www.c-sharpcorner.com/article/C-Sharp-heaping-vs-stacking-in-net-part-i/)

[Garbage Collection Fundamentals](https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/fundamentals)

## Classes Notes

C# classes are used to define objects that have state (fields) and behavior (methods).
The class keyword is used to declare a new class.
Classes can have fields, properties, methods, and events.
Fields are used to store data within a class.
Properties provide a way to access and modify the data stored in fields.
Methods define the behavior of a class and can be used to perform actions or return values.
Constructors are special methods used to initialize objects of a class.

## Constructor Notes

When an instance of a class is created, its **constructor** is called.
A class or struct may have multiple constructors that take different arguments.

Constructors allow us to set default values, limit instantiation, and write code that is flexible and easy to read.

A constructor is a method whose name is the same as the name of its type.

        public class Person
        {
        private string last;
        private string first;

        public Person(string lastName, string firstName)
        {
            last = lastName;
            first = firstName;
        }

        // Remaining implementation of Person class.
        }

## Properties Notes

A **property** is a member that provides a flexible mechanism to read, write, or compute the value of a private field.

Properties can be used as if they're public data members, but they're special methods called accessors.

Properties can be read-write (they have both a get and a set accessor), read-only (they have a get accessor but no set accessor), or write-only (they have a set accessor, but no get accessor). Write-only properties are rare and are most commonly used to restrict access to sensitive data.

## Stack and Heap

The stack and heap help us run code.

They reside in the operating memory on our machine and contain the pieces of info to make it happen.

The Stack is more or less responsible for keeping track of what's executing in our code (or what's been "called").  The Heap is more or less responsible for keeping track of our objects (our data, well... most of it - we'll get to that later.).

Once we complete the first box of code, we move down and get rid of the previous box from the stack. (Stack)

Heap is similar, except its purpose is to hold information.

With the Heap, there are no constraints as to what can be accessed like in the stack. 

Value Types

In C#, all the "things" declared with the following list of type declarations are Value types (because they are from System.ValueType):

    bool
    byte
    char
    decimal
    double
    enum
    float
    int
    long
    sbyte
    short
    struct
    uint
    ulong
    ushort

Reference Types

All the "things" declared with the types in this list are Reference types (and inherit from System.Object... except, of course, for object which is the System.Object object):

    class
    interface
    delegate
    object
    string

## Garbage Collection Fundamentals

This serves as an automatic memory manager.

The garbage collector manages the allocation and release of memory for an application. Therefore, developers working with managed code don't have to write code to perform memory management tasks. 

## Questions

1. What’s the difference between a static and an instance constructor?
2. How does the use of a static constructor differ from setting properties/values?
3. Knowing what you now know about the stack and the heap, how might you rethink the way you did projects in previous courses, to make more effecient use of memory?
4. Compare “Garbage Collection” in C# with the lifecycle of normal household items.

## Answers

1. Static constructors allow you to initialize variables in a class. Instance constructors are what you call whenever you crate new objects.
2. Static constructor initializes static members, and properties and values initializes non-static members.
3. I would use the stack more often for storing local variables so I could free up heap memory for storing objects that need to be persistent for longer periods of time.
4. Its like buying a new item, and once its use is used up, we discard it. We do this often to reduce clutter.

## Things I want to know more about

I want to understand more in depth the cycle of garbage collection.
I want to know more about the best practices while programming so we efficiently use memory space.