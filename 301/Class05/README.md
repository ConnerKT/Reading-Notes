# Putting it all Together

This topic is important to me because I want to be able to apply the skills I've learned so far and make a concise collection of my knowledge.

## [Retrospective 5](https://connerkt.github.io/Reading-Notes/301/Class05/Retro05)

## References

<https://reactjs.org/docs/thinking-in-react.html>.

<https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK>.

## Thinking in React

When building applications in React, its best to think of the structure of the program before.
You want to break it into pieces, components.
You'll create your states.
Then you connect your components together so data flows between them.

Make a static version of your web page first, so you can visualize on how to make it interactive.

## Thinking of React Questions

1. What is the single responsibility principle and how does it apply to components
2. What does it mean to build a ‘static’ version of your application?
3. Once you have a static application, what do you need to add?
4. What are the three questions you can ask to determine if something is state?
5. How can you identify where state needs to live?

## Thinking of React Answers

1. When in components its best to keep them simple, and if it keeps growing to break it into sub components.
2. A live viewable version, just probably not with features.
3. You start working on the logic, you need to make your states.
4. Does it change over time? Does the product need to show up for user input? Does your item need to be rerendered?
5. Putting it directly into their common parent.

## Higher-Order Functions

**Higher-Order Functions** are functions that operate on other functions, either by taking them as arguments or by returning them.

They allow us to abstract over actions, not just values.

It can help us create new functions.
It can help us change other functions.
We can even write functions that provide new types of control flow.

**In Javascript, functions can be assigned to variables in the same way that strings or arrays can. They can be passed into other functions as parameters or returned from them as well.**

**A “higher-order function” is a function that accepts functions as parameters and/or returns a function.**

## Higher-Order Questions

1. What is a “higher-order function”?
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
3. Explain how either map or reduce operates, with regards to higher-order functions.

## Higher-Order Answers

1. A “higher-order function” is a function that accepts functions as parameters and/or returns a function.

2. Its returning a function m > n

3. Map is a glorified for loop that loops through an array.

## Things I want to know more about

I want to understand on the best ways and reasons you would use a higher order function.
I want to understand when this will be needed in my career.