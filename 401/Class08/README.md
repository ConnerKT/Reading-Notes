# Collections & Enums

This topic is important to me because I want to understand the deeper concepts of C#, and other programming languages.

## [Retrospective 8](https://connerkt.github.io/Reading-Notes/401/Class08/Retro08)

## References

[Collections](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/collections)
[Enums](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/enum)

## Collections

Collections are data structures that allow you to group and store multiple elements of the same or different types. They provide various methods and properties for manipulating and accessing the elements they contain. In C#, collections are implemented through classes found in the System.Collections and System.Collections.Generic namespaces.

Common types of collections in C# include:

    Lists: An ordered collection that allows duplicate elements. Lists are dynamically resizable arrays.
    Arrays: A fixed-size collection of elements of the same type.
    Dictionaries: A collection of key-value pairs, where each key must be unique.
    Sets: An unordered collection of unique elements, meaning duplicates are automatically excluded.
    Queues: A collection that follows the First-In-First-Out (FIFO) principle.
    Stacks: A collection that follows the Last-In-First-Out (LIFO) principle.

Example of a List in C#:

    using System;
    using System.Collections.Generic;

    public class CollectionsExample
    {
        public static void Main()
        {
            List<int> myNumbers = new List<int>();
            myNumbers.Add(1);
            myNumbers.Add(2);
            myNumbers.Add(3);

            foreach (int number in myNumbers)
            {
                Console.WriteLine(number);
            }
        }
    }

## Enums

Enums (short for enumerations) are a set of named constants representing integral values. They allow you to define symbolic names for a set of related integral values to make your code more readable and maintainable. Enums are useful when you have a fixed set of options or states for a variable.

Ex.

    public enum DaysOfWeek
    {
        Sunday,
        Monday,
        Tuesday,
        Wednesday,
        Thursday,
        Friday,
        Saturday
    }

    DaysOfWeek today = DaysOfWeek.Monday;

By default, enums are assigned integral values starting from 0, but you can explicitly set the values as shown above.

Enums are handy for representing state, options, or choices in your code and help you avoid using "magic numbers" or "magic strings" that can lead to errors and reduce code clarity.