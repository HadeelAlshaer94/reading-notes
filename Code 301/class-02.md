# Code 301 - Intermediate Software Development
## State and Props

React lets you define components as classes or functions. Components defined as classes currently provide more features which are described in detail on this page. 

![image](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

 >The only method you must define in a React.Component subclass is called render(). All the other methods described on this page are optional. 
# What are component lifecycle events?

 ## Mounting
When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.
## Updating
Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps
## Unmounting
The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.
## constructor()
The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance

# Static getDerivedStateFromProps() :

getDerivedStateFromProps(props, state) is a static method that is called just before render() method in both mounting and updating phase in React. It takes updated props and the current state as arguments. We have to return an object to update state or null to indicate that nothing .

# render():
  React component lifecycle and is called by React at various app stages, generally when the React component is first instantiated, or when there is a new update to the component state 
# componentDidMount() :
 
  The componentDidMount() method allows us to execute the React code when the component is already placed in the DOM (Document Object Model). This method is called during the Mounting phase of the React Life-cycle i.e after the component is rendered

# shouldComponentUpdate() :
 The default behavior in react is to rerender after every state change. Setting shouldComponentUpdate() to false allows you to prevent this from happening. This is in order to optimize performance. 

 # getSnapshotBeforeUpdate() :
 
 
What is React getSnapshotBeforeUpdate

Since the release of React Suspense, rendering components are becoming more asynchronous.

This is a good thing for folks with limited bandwidth or weak devices.



#  componentWillUnmount() 
The componentWillUnmount() method allows us to execute the React code when the component gets destroyed or unmounted from the DOM (Document Object Model). This method is called during the Unmounting phase of the React Life-cycle i.e before the component gets unmounted.

All the cleanups such as invalidating timers, canceling network requests, or cleaning up any subscriptions that were created in componentDidMount() should be coded in the componentWillUnmount() method block.
# Linked List 
Linked List is the structure where all elements are arranged in linear order, which is determined by pointer stored in each element.


## What types of things can you pass in the props?
What Are Props? Props (aka "properties") in React allows us to pass values from a parent component down to a child component. The values can be any data type, from strings to functions, objects, etc.

## What is the big difference between props and state?

The key difference between props and state is that state is internal and controlled by the component itself while props are external and controlled by whatever renders the component.

## When do we re-render our application?
React components automatically re-render whenever there is a change in their state or props. A simple update of the state, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.

## What are some examples of things that we could store in state?

State inside a React component is the encapsulated data that is persistent between renderings. useState() is the React hook responsible for managing state inside a functional component. I like that useState() indeed makes the work with state quite easy.

### The Data Flows Down
Neither parent nor child components can know if a certain component is stateful or stateless, and they shouldn’t care whether it is defined as a function or a class.

This is why state is often called local or encapsulated. It is not accessible to any component other than the one that owns and sets it.