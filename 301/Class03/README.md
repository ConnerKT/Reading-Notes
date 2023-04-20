# Passing Functions as Props

This topic matters to me because I want to deeply connect different functions and components to have a codebase that is clean, well built, and manageable.

## [Retrospective 3](https://connerkt.github.io/Reading-Notes/301/Class03/Retro03)


## References

<https://reactjs.org/docs/lists-and-keys.html>.
<https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab>.
<https://www.youtube.com/watch?v=c05OL7XbwXU>.
<https://reactjs.org/tutorial/tutorial.html>.
<https://reactjs.org/docs/lifting-state-up.html>.


## List and Keys

To transform list its like using the map() method to double a given array into another array.

You can build collections of elements and include them in JSX using curly braces {}.

Usually you would render lists inside a component.

A **Key** is a special string attribute you need to include when creating lists of elements.

Keys help React identify which items have changed, are added, or are removed.

React defaults to using indexes as keys, but its not recommended.

## Lists and Keys Questions

1. What does .map() return?
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
3. Each list item needs a unique ____.
4. What is the purpose of a key?

## Lists and Keys Answers

1. It returns an array, with the same amount of numbers as the previous array.
2. You can use the map method, and create an element to contain each index of that loop.
3. key.
4. To help react identify which items have changed.

## The Spread Operator

The **Spread Operator** is a useful and quick syntax for adding items to arrays, combing arrays or objects, and spreading an array out into a function's arguments.

Spread Syntax - the use of the three dots (...) to expand an iterable object into the list of arguments.

(When ...arr is used in the functiomn call, it 'expands' an iterable object arr into the list of arguments).

The spread sytnac 'Spreads' the array into serpate arguments.

Theres a lot of functions it can do such as:
    Copying an array
    Concatenating or combining arrays
    Using Math functions
    Using an array as arguments
    Adding an item to a list
    Adding to state in React
    Combining objects
    Converting NodeList to an array



## The Spread Operator Questions

1. What is the spread operator?
2. List 4 things that the spread operator can do.
3. Give an example of using the spread operator to combine two arrays.
4. Give an example of using the spread operator to add a new item to an array.
5. Give an example of using the spread operator to combine two objects into one.

## The Spread Operator Answers

1. The spread operator is a operator that spreads an array into seperate arguments.
2. Copying an array, combining arrays, using math functions, and combining objects.
3. Ex. newArray = ...OldArray (this is contained in an array)
4. Using the spread operator to add multiple arrays together
    Ex. newArray = ...thisarray, ...otherarray
5. For example

        let products = {
            ...oldproducts
            ...newproducts
        }

## How to Pass Functions Between Components Questions

1. In the video, what is the first step that the developer does to pass functions between components?
2. In your own words, what does the increment function do?
3. How can you pass a method from a parent component into a child component?
4. How does the child component invoke a method that was passed to it from a parent component?

## How to Pass Functions Between Components Answers

1. Create a function.
2. The increment function takes in a name and if the array name matches the name of the one thats passed through, change its count by one.
3. Props
4. Using it props.method.

## Things I want to know more about

I want to know more about how to apply these in components and how essential it is.
