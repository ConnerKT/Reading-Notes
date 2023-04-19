# State and Props

## [Retrospective 2](https://connerkt.github.io/Reading-Notes/301/Class02/Retro02)

## References

<https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093>.
<https://www.youtube.com/watch?v=IYvD9oBCuJI>.
<https://reactjs.org/docs/state-and-lifecycle.html>.
<https://reactjs.org/docs/handling-events.html>.
<https://reactjs.org/tutorial/tutorial.html>.
<https://react-bootstrap.github.io/>.
<https://getbootstrap.com/docs/5.0/examples/cheatsheet/>.
<https://bootstrapshuffle.com/classes>.
<https://www.netlify.com/>.

## React Lifestyle

**Lifestyle events** are methods you can use on components.

They are called during the lifecycle of a component, and allow you to update the UI and the application states.

The Three Phases are:
1. Mounting
2. Updating
3. Unmounting

## Phases of a Component Lifestyle

**Mounting** : When an instance of a component is being created and inserted into the DOM.

Life of Lifestyle Events for Mounting:

    Constructor
    static 
    getDerivedStateFromProps
    render
    componentDidMount
    UNSAFE_componentWillMount

**Updating**: Anytime a component is updated or state changes then its rerendered.

List of Lifestyle Events for Updating:

    static getDerivedStateFromProps
    shouldComponentUpdate
    render
    getSnapshotBeforeUpdate
    componentDidUpdate
    UNSAFE_componentWillUpdate
    UNSAFE_componentWillReceiveProps

**Unmounting** : Lastly, when the a component is being removed from the DOM.

The only lifecycle event is:

    componentWillUnmount

The **Constructor** for a React component is called before it is mounted.

If the component is a subclass you should call super(props). or props will be undefined.

Constructors can be used to assign state or to bind event handle methods to an instance.

**Render()** is the only required method in a class component.a

## React Lifestyle Questions

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
2. What is the very first thing to happen in the lifecycle of React?
3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
4. What does componentDidMount do?

## React Lifestyle Answers

1. Render
2. The Mounting.
3. Constructor, Render, ComponentDidMount, React Updates, ComponentWillUnmount
4. Used to load anything using a network request or initialize the DOM.

## React State VS Props Questions

1. What types of things can you pass in the props?
2. What is the big difference between props and state?
3. When do we re-render our application?
4. What are some examples of things that we could store in state?

## React State VS Props Answers

1. Any Data Type
2. Props you pass in, state is handled inside that component.
3. State re-renders our app.
4. State helps to continue to update, to store the updated value/content.
