# State and Props

## React lifecycle
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

    render

2. What is the very first thing to happen in the lifecycle of React?

   Mounting

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
    1. constructor
    2. render 
    3. componentDidMount
    4. React Updates
    5. componentWillUnmount
4. What does componentDidMount do?

    This method initialize the DOM and load load anything using a network request.

## React State Vs Props
1. What types of things can you pass in the props?

   We pass props as an argument it can be strings or numbers.


2. What is the big difference between props and state?

    The big difference is that we can pass props into a component it is handled out side the component but state is handled inside that comopnent.

3. When do we re-render our application?
 
    When we change the state inside it.

4. What are some examples of things that we could store in state? 

    input element and checkbox