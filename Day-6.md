## What is an event in react?

An event is an action that could be triggered as a result of the user action or system generated event. For example, a mouse click, loading of a web page, pressing a key, window resizes, and other interactions are called events.

React has its own event handling system which is very similar to handling events on DOM elements. The react event handling system is known as Synthetic Events. The synthetic event is a cross-browser wrapper of the browser's native event.

camelCase Convention: Instead of using lowercase we use camelCase while giving names of the react events. That simply means we write ‘onClick’ instead of ‘onclick’.

Pass the event as a function: In React we pass a function enclosed by curly brackets as the event listener or event handler, unlike HTML where we pass the event handler or event listener as a string.

Prevent the default: Just returning false inside the JSX element does not prevent the default behavior in react. Instead, we have to call the ‘preventDefault’ method directly inside the event handler function.

on mouse hovrngs some actions will be triggered

## What is memory leak and how to overcome?

Memory leak occurs when programmers create a memory in heap(call stack) and forget to delete it.

The consequences of memory leak is that it reduces the performance of the computer by reducing the amount of available memory. Eventually, in the worst case, too much of the available memory may become allocated and all or part of the system or device stops working correctly, the application fails, or the system slows down vastly .

Memory leaks are particularly serious issues for programs like daemons and servers which by definition never terminate.

overcome - use useEffect cleanup flag boolean flag useEffect clenup Abort Controler

## Do you prefer function-based or class component and why ?

Functional Component. A functional component is just a plain JavaScript pure function that accepts props as an argument and returns a React element(JSX). A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.


## Explain reducer as pure function in redux

In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action. (previousState, action) => newState

. A reducer is a pure function that determines changes to an application’s state. Reducer is one of the building blocks of Redux.

### USES OF REDUX: With the help of redux it is easy to manage state and data.

REDUCER: In redux, the reducers are the pure functions that contain the logic and calculation that needed to be performed on the state. These functions accept the initial state of the state being used and the action type. It updates the state and responds with the new state. This updated state is sent back to the view components of the react to make the necessary changes.

Pure function: A function is said to be pure if the return value is determined by its input values only and the return value is always the same for the same input values or arguments. A pure function has no side effects. Below is an example of a pure function:

const multiply= (x, y) => x * y; multiply(5,3);

Reducers are pure functions hence they cannot do the following things:–.
It cannot change or access any global variables. It cannot make any API calls. It cannot call any impure function in it like date or random

## Why do we use redux thunk?

The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API. Redux Thunk is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. One of the main use cases for this middleware is for handling actions that might not be synchronous, for example, using axios to send a GET request.

redux middleware called thunk. It allows us to return functions instead of objects from redux actions. Plain redux doesn’t allow complex logic inside action functions, you can only perform simple synchronous updates by dispatching actions.

This middleware extends its ability and lets you write complex logic that interacts with the store. Thunk doesn’t interfere with the action until it returns a function. Thunk allows us to dispatch actions manually, which gives us the power to incorporate some logic or run some asynchronous code before dispatching an action. The function returned from action is called a thunk function which is called with two arguments :

dispatch: It is a method used to dispatch actions, that can be received by reducers.
getState: It gives access to store inside the thunk function.
A thunk function may contain any arbitrary logic, sync, or async, and can call dispatch or getState at any time. Before moving any further let’s understand the difference between the flow of redux with and without thunk.

## What do you know about NPM?

NPM stands for 'Node Package Module',npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.
npm consists of three distinct components:

the website the Command Line Interface (CLI) the registry

NPM stands for the node package manager, npm is used for node dependency management. Most of the time, we use npm as a server-side node dependency tool.
NPM gets installed with NodeJs installation.
NPM uses nested dependencies, so we can use different versions of any module in our code. Nested dependencies mean that any dependency is again dependent on another dependency, which creates huge amounts of data but makes our codebase clean and reduces unwanted errors.
There may be a npm version conflict, so nested dependencies are used to resolve the npm version conflict.
NPM has a special tool for handling and managing all packages, so this is an advantage here.
NPM does have stability, so if you create a high load in the application that manages all the work of packages.
The npm approach common Js modules and they use explicit Dependency Injection.