## What is UseMemo Hook ?(Implementation)

The useMemo is a hook used in the functional component of react that returns a memoized value. In Computer Science, memoization is a concept used  when we don’t need to recompute the function with a given argument for the next time as it returns the cached result.

 A memoized function remembers the results of output for a given set of inputs.

ex:- 1+2=3 ,whn we enter same input again it give catched value without doing the addition
The useMemo hook is used to improve performance in our React application.

## What is UseRef Hook ?(Implementation)

The useRef is a hook that allows to directly create a reference to the DOM element in the functional component.

The useRef returns a mutable ref object. This object has a property called .current. 

The value is persisted in the refContainer.current property. These values are accessed from the current property of the returned object. The current property could be initialised to the passed argument initialValue e.g. useRef(initialValue). The object can persist a value for a full lifetime of the component.

## What is Context api

The Context API provides a way to pass data through the component tree without having to pass props down manually at every level. The syntax is really easy to understand and also, there is not much boilerplate code to write to get it set up.

Provider The Provider component is going to be used to wrap the components that are going to have access to our context. The Provider component receives a prop called value, which can be accessed from all the components that are wrapped inside Provider, and it will be responsible to grant access to the context data

Consumer After you wrap all the components that are going to need access to the context with the Provider component, you need to tell which component is going to consume that data. 


## Difference between callback and useCallback Hook ?

callback is a  fun that is called after certain interval of time or when required
The callbacks are needed becaouse JS is an event driven language that means instead of waiting for a task to be completed it will keep executing other task. 

The callback function may be some code that hasn't been executed yet, and you don't know what's above your function in the call stack

The useCallback hook is used when you have a component in which the child is rerendering again and again without need.

Pass an inline callback and an array of dependencies. useCallback will return a memoized (function call) version of the callback that only changes if one of the dependencies has changed.

prevent unnecessary renders.

const memoizedCallback = useCallback( () => { doSomething(a, b); }, [a, b], );

## What is Props Drilling Concept ?What is State Uplifting ?

Props:-Components in React can be passed some parameters. These parameters are generally named props.

Prop drilling is basically a situation when the same data is being sent at almost every level due to requirements in the final level.

The problem with Prop Drilling is that whenever data from the Parent component will be needed, it would have to come from each level, Regardless of the fact that it is not needed there and simply needed in last.

A better alternative to this is using useContext hook. The useContext hook is based on Context API and works on the mechanism of Provider and Consumer.
 Provider needs to wrap components inside Provider Components in which data have to be consumed. Then in those components, using the useContext hook that data needs to be consumed.

Lifting up the State

every component in React has its own state. Because of this sometimes data can be redundant and inconsistent. 
So, by Lifting up the state we make the state of the parent component as a single source of truth and pass the data of the parent in its children.


## Difference between useEffect and useContext ?

React Hooks allow us to manage state data inside functional components; now we don’t need to create class components just to manage state data.

React has a few built-in hooks such as useState, useCallback, useEffect, etc.

useContext: useContext is a hook that provides a way to pass data through the component tree without manually passing props down through each nested component.

useEffect: A hook that helps us to perform mutations, subscriptions, timers, logging, and other side effects after all the components has been rendered. 
The useEffect accepts a function that is imperative in nature and a list of dependencies. When its dependencies change it executes the passed function.

Now if we don’t use useEffect, every time a button is pressed data will be fetched from the server even if the choice does not change. In such a condition this hook helps us to not call the fetching logic unless our choice changes.