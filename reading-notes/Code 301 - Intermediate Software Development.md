
# NOTES 
## Reading 01 
### Intro to React and Components
- a compononet is similar to functions in that it is a building block of code using the react app.
- each component could have other component or styling, html. moreover, component could have arguments passed and those are called props. finally, the react app component returns react elements that describe how user interface should apear. moreover, components use es6 class syntax (my thoughts: you can interchange js classes with react component syntax. although, doesn't seem that component deviate in syntax from js since its a framework.). they are referred to as class, smart, stateful, container. this is very helpful because people do use different language to describe react components.
need to manage local state

  1. need to add lifecycle methods to your component

  2. need to add logic for event handlers

  3. Otherwise, always use a functional component

- advantages: data flow in react is unidirectional
    1. The view is a result of the application state. State can only change when actions happen. When actions happen, the state is updated.
    2. so data flow in react is cyclical and dependant in each component.
    3. components and subcomponents are generally aggregated relationship.
props are short for properties
they are passed in as arguments and the components are using the props in a aggregated relationship.
flow is unidirectional and is passed in from and used from call of another component.
