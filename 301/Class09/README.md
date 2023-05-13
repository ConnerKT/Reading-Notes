# Functional Programming

This topic is important to me because I want to create programs that aren't prone to errors, and build applications that are well formated.

## [Retrospective 9](https://connerkt.github.io/Reading-Notes/301/Class09/Retro09)

## References

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa).
[Node.Js Tutorial (Modules and require())](https://www.youtube.com/watch?v=xHLd36QoS4k).

### Functional Programming Notes

**Functional Programming** is a programming style that views computation as the evaluation of mathematical functions and avoids using mutable data or changing the program's state.

The first concept is **pure functions**.

To define what a **pure function** is, you have to see if its:

1. It returns the same result if given the same arguments
2. It does not cause any observable side effects.

If our function reads external files, its not pure. (the files can be changed)

If a function relies on a random number gen, it cannot be pure.

Another concept is **Immutability**.

Its when its unchanging over time or unable to be changed.

When data is immutable, its ate cannot change after it's created. If you want to change an immutable object, you don't. You just create a new object with the new value.

Another concept is **Referential Transparency**.

This is a property of a function that consistently produces the same output for the same input and has no side effects.

### Functional Programming Questions

1. What is functional programming?
2. What is a pure function and how do we know if something is a pure function?
3. What are the benefits of a pure function?
4. What is immutability?
5. What is Referential transparency?

### Functional Programming Answers

1. A programming way, that emphasizes the use of pure functions and immutable data.
2. A function that consistently produces the same output for the same input and has no side effects.
3. Modularity, Reusable code , and more.
4. An object that has a state that cannot be modified.
5. This is when a function produces the same output for the same input and has no side effects.

## Node.js for Beginners (Module and Require) 

When we write a Node.js App, we split our code in different modules.

Then we call on these modules when we need them.

We would make other 'modules' so we can require them to other JS, or code files, so we can keep our code clean and organized.

You would make a file and make it as a function, then we would require the function into our other file.

## Node.js for Beginners (Module and Require) Questions

1. What is a module?
2. What does the word ‘require’ do?
3. How do we bring another module into the file the we are working in?
4. What do we have to do to make a module available?

## Node.js for Beginners (Module and Require) Answers

1. A module is containment of code that keeps functions in so we can reuse them in the future.
2. It allows us to import other code(like libraries) into our code.
3. You would require the file at the top of your code (require(./file))
4. You have to state in your module what you want to export out of it

## Things I want to know more about

I want to know how to use pure functions in my own code, and the best practices.

I want to learn how to get better with making code that is reusable, and concise.
