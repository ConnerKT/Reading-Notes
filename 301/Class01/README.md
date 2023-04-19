# Introduction to React and Components

## [Retrospective 1](https://connerkt.github.io/Reading-Notes/301/Class01/Retro01)

This topic is important to me because I want to be able to create apps with great UI where the user feels welcomed.

## References

<https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm>.

<https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child>.

<https://reactjs.org/tutorial/tutorial.html>.

<https://reactjs.org/docs/hello-world.html>.

<https://reactjs.org/docs/introducing-jsx.html>.

<https://reactjs.org/docs/rendering-elements.html>.

<https://reactjs.org/docs/components-and-props.html>.

## Component-Based Architecture

**Component-based architecture** focuses on the decomposition of the design into individual functional or logical components that represent well-defined communication interfaces containing methods, events, and properties.

Provides a higher level of abstraction and divides the problem into sub problems.

Main Objective is to insure **component reusability**.

Component-oriented vs Object-oriented

Component-oriented has reduced time in market, and development cost by reusing existing components.
Increased reliability with the reuse of the existing components as well.

### Components

A **Component** is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

**Component** is a software object, intended to interact with other components.

A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties.

### Views of a Component

Object-Oriented view:

Viewed as a set of one or more cooperating classes.

Conventional View:

Viewed as a functional element or a module of a program that integrates the processing logic, internal data structures, and interface.

Process-related view:

In this view, it isn't made from scratch, but from a library of existing components.

### Characteristics of Components

Reusability, Replaceable, Not content specific, Extensible, Encapsulated, and Independent.

Remember to follow the Principles of Component-Based Design and the Guidelines.

## Component-Based Architecture Questions

1.What is a “component”?
2.What are the characteristics of a component?
3.What are the advantages of using component-based architecture?

## Component-Based Architecture Answers

1. A component is a software object, that can be reused and can interact with other components.
2. It's reusable, replaceable, Independent.
3. Making code that can be deployed quickly and lowering the development cost.

## What is Props and How to Use it in React

React has a different approach to data flow and manipulation than other frameworks.

## Props

**React** is a component-based library that divides the UI into little reusable pieces. Sometimes components need to communicate(send data to eachother) and the way to pass data between components is by using **Props**

**Props** stands for properties and is being used for passing data from one component to another.

Data with Props is being passed in a uni-directional flow (one way from parent to child).

Props data is read-only, which means that data coming from the parent should not be changed by child components.

## Props step by step

1. Define an atrribute and its value
2. Then pass it to child components by using props
3. Render the Props data



## What is Props and How to Use it in React Questions

1.What is “props” short for?
2.How are props used in React?
3.What is the flow of props?

## What is Props and How to Use it in React Answers

1. Properties
2. It is used to pass attribute and value to a child and render the data
3. Uni-directional

## Things I want to know more about

I want to understand in depth on how to pass the data to children.
I want to learn how to utilize this in a complex coding environment.


