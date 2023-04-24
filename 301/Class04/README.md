# React and Forms Notes!

This topic is important to me because I want to understand the concept of having user inputs be used on my site, and also managing state iwth that.

## [Retrospective 4](https://connerkt.github.io/Reading-Notes/301/Class04/Retro04)

## References

<https://reactjs.org/docs/forms.html>.

<https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff>.

<https://react-bootstrap.github.io/forms/overview/>.

<https://reactjs.org/docs/conditional-rendering.html>.

## React Docs - Forms

Imperative Programming is how you implement interaction. You have to command each element.

Using react you don't directly manipulate the UI.

You declare what you want to show, and React figures out how to update the UI.

To make a form in React, its different. We have to take in different things into consideration. 
State allows us to have a form of in memory.

You can trigger state updates in response to two kinds of inputs:

1. Human inputs.

2. Computer inputs (network response arriving, timeout, image loading)

Using State variables to update the UI.

You need to start with the states that are definitely needed, and then create the others.

Ex. A state that takes in an answer, and also a state that has an error.

Event Handlers will usually take in a a user input.

## React Docs Questions

1. What is a ‘Controlled Component’?
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
3. How do we target what the user is entering if we have an event handler on an input field?

## React Docs Answers

1. A component that is controlled by React state.
2. Every time they type so we can get a constant reactive input.
3. We can apply it to the state, to react to what the user is inputing.

## The Conditional Ternary Operator

The Ternary operator lets us shorten our if statements into one line of code.

Like an if statement, the conditional ternary is just a shorthand version of it.

The ? serpates our conditonal form from our true value, anything between the ? and the : is what is executed if the condition evaluates to true.

The : is the else for the program.

    condition ? value if true : value if false

## The Conditional Ternary Operator Questions

    1. Why would we use a ternary operator?

    2. Rewrite the following statement using a ternary statement:

    if(x===y){
      console.log(true);
    } else {
      console.log(false);
    }

## The Conditional Ternary Operator Answers

1. We would use a ternary operator to help shorten your if statements into a more clean and precise code.

        2. x === y ? console.log(true) : console.log(false)

## Things I want to know more about

I want to know more about applying states in a deeper user input area.
 I want to know how complex it can get.