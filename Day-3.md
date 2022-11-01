## Difference between Axios and fetch

One of the fundamental tasks of any web application is to communicate with servers through the HTTP protocol. This can be easily achieved using Fetch or Axios. Fetch and Axios are very similar in functionality.
---- Fetch:-

The Fetch API provides a fetch() method defined on the window object.

It also provides a JavaScript interface for accessing and manipulating parts of the HTTP pipeline (requests and responses).

The fetch method has one mandatory argument- the URL of the resource to be fetched.

This method returns a Promise that can be used to retrieve the response of the request.

fetch('path-to-the-resource-to-be-fetched') .then((response) => {

// Code for handling the response }) .catch((error) => {

// Code for handling the error });

Fetch has no url in request object.

Fetch is built into most modern browsers; no installation is required as such.

Fetch uses the body property.

Fetch’s body has to be stringified.

Fetch is a two-step process when handling JSON data- first, to make the actual request; second, to call the .json() method on the response.

Fetch only supports Chrome 42+, Firefox 39+, Edge 14+, and Safari 10.1+ (This is known as Backward Compatibility).

---- Axios:-

Axios is a Javascript library used to make HTTP requests from node.js or XMLHttpRequests from the browser .

It supports the Promise API that is native to JS ES6. - It can be used intercept HTTP requests and responses and enables client-side protection against XSRF.

It also has the ability to cancel requests.

axios.get('url') .then((response) => {

// Code for handling the response }) .catch((error) => {

// Code for handling the error })

Axios has url in request object.

Axios is a stand-alone third party package that can be easily installed.

Axios enjoys built-in XSRF protection.,fetch doesnt

Axios uses the data property.

Axios data contains the object.

Axios performs automatic transforms of JSON data.

Axios has wide browser support.

## What is UseState Hook ?(Implementation)

The useState() is a Hook that allows you to have state variables in functional components .
Class components have state and lifecycle methods: class Message extends React.
The useState hook is a special function that takes the initial state as an argument and returns an array of two entries.
Syntax: The first element is the initial state and the second one is a function that is used for updating the state.
const [state, setState] = useState(initialstate)

To use useState you need to import useState from react
import React, { useState } from "react"



## What is useEffect Hook ?(Implementation)

useEffect Hook is to eliminate the side-effects of using class-based components.
For example, tasks like updating the DOM, fetching data from API end-points, setting up subscriptions or timers, etc can be lead to unwarranted side-effects.



## What is UseReducer Hook ?(Implementation)

The useReducer Hook is the better alternative to the useState hook
It is generally more preferred over the useState hook when you have complex state-building logic or when the next state value depends upon its previous value or when the components are needed to be optimized.
The useReducer hook takes three arguments including reducer, initial state, and the function to load the initial state lazily.
const [state, dispatch] = useReducer(reducer, initialArgs, init);