
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

## Reading 02
### State and Props

1. Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?
    ****
   1. **During the mounting process, render is called before componentDidMount.**
   2. React lets you create components as functions or classes.
   3. mounting, updating, and unmounting are key states of component lifecycle.
   4.  Mounting phase - an instance of a component is being created and inserted into the DOM.
   5.  Updating - it is state changes or  rerendered is done in the oreder: 
       1.  static getStateFromProps, shouldCOmponentUPdate, render,
       2.  getSnapshotBeforeUPdate, componentDidUPdate, UNSAFE_componentWillUpdate, UNSAFE_compnentWillReceiveProps
   6. Unmounting - component is being removed.
   7. 
   ****
2. What is the very first thing to happen in the lifecycle of React?
   ****
   1. **Constructor gets called first during the creation of component. further, super gets called if at subcomponent.**
   2. (needs further evaluation) according to the source reading, the constructor is very similar to how classes are built as far as scope for constructors. So, if a there is a inheritence relationship, then the child is responsible for calling the parent constructor using the keyword super(x,x,x,freestuff, freestuff, freestuff). Note: props will be passed and have access to props: super(props)
   3.  this.state is a can be assigned here in constructor. Note: Field Declarations available?
   4.  avoid this.setState() in constructor. this will ignore all updates and cause unwanted side effects.
   5.  static (mutable) getDerivedStateFromProps() is used in case state relies on chages in props over time.

    ****
3. What does componentDidMount do?
   ****
   1. **loads network request or initialize the DOM**
   2. this method gets invoked immediately after component is mounted
   3. loads network request or intitialize DOM
   4. useful for usage of subsriptions and must componentWillUnmount() any subscriptions when unsubscribing.
   **** 

4.  what types of things can you pass in the props? 
    ****
    1. **Props can be treated as arguments/parameters that will want to pass information.**
    2. is this similar to props or state?

    ****


5.  what is the gig difference between props and state?
    ****
    1.  props are handled outside of component. aggregation relationship
    2.  states are in scope inside the component. composition relationship

    ****
6.  when do we re-render our application?
    ****
    1.  **changing state but not for props. state will re- render the application.**
    ****

## Reading 03
### Passing Functions as Props
****
### Arrays.prototype.map() notes in ReactJS
**** 
1. map() is a prototype of Arrays class (Arrays.prototype.map()). thus, the return is returning an array.
2. inside the body of a tag, if we use {someName} then we can display the contents in someName onto the screen.
3. each list item needs to have a unique **key**. 
4.  Keys help react identify which items have changed. keys should be given to the elements inside the array .
****
Spread Operator ...
****
1. Spread Syntax can be used when all elements from an object or array need to be included in a list. very similar to english elipse ... where i can say 1, 2, 3, ..., 10. we can assume that the elipse says there are integers that should be included. 
2. pass in arguments to a function, pass to array literals, and pass object to copy another object.
3. first, we can do something like newArr = [...arrOneToTen, 11,12] where arrOneToTen will assign all elements into the newArr. second example, if a function x(...aArrayParam, y) we can assign parameters using spread operator.
4. to clone a object all we do is: cloneObj = {...obj} and all the key:values paris will be assigned to cloneObj



## Reading 04
### React and Forms
- What is a Controlled Component?
  - setState will make state mutable within their own state based on user input with input, textarea, select, kind of tags.
- we should always wait for the user response when they submit the for
- target with multiple inputs from user by adding attribute to each element. handler function will choose what to do based on event.target.
### Ternary Operator
- a boolean value or truthy, falsy is needed. so then ? will do x?if:else
- x===y ? console.log(true) : console.log(false)

****
## Reading 05
### Putting it All Together
****
1.  what is the **single responsibility principle** and how does it apply to components?
    - coding components into a focused reason.
2.  What does it mean to build a ‘static’ version of your application?
    - static is building the UI but has no interactivity.   
3.  Once you have a static application, what do you need to add?
    - library, FilterProductTable, dont use state.   
4.  What are the three questions you can ask to determine if something is state? 
    -   Is it passed in from a parent via props? If so, it probably isn’t state.
    -   Does it remain unchanged over time? If so, it probably isn’t state.
    -   Can you compute it based on any other state or props in your component? If so, it isn’t state.
5.  How can you identify where state needs to live?
    -   **FilterableProductTable**
    -   ProductTable needs to filter the product list based on state and SearchBar needs to display the search text and checked state.
    -   The common owner component is FilterableProductTable.
    -   It conceptually makes sense for the filter text and checked value to live in FilterableProductTable

****

