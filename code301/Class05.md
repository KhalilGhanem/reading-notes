# Putting it all together

##React Docs - thinking in React

1. How would you break a mock into a component heirarchy?

    we can break mocks by draw boxes around every component (and subcomponent).

2. What is the single responsibility principle and how does it apply to components?

    a component should ideally only do one thing.

3. What does it mean to build a ‘static’ version of your application?

    That we build and renders the UI without interactivity in the site.

4. Once you have a static application, what do you need to add?

    Adding states.

5. What are the three questions you can ask to determine if something is state?

    * Is it passed in from a parent via props?
    * Does it remain unchanged over time?
    * Can you compute it based on any other state or props in your component?

6. How can you identify where state needs to live?

    * Identify every component that renders something based on that state.
    * Find a common owner component (a single component above all the components that need the state in the hierarchy).
    * Either the common owner or another component higher up in the hierarchy should own the state.
    * If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.