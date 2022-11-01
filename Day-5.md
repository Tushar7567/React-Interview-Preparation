Do you know about SEO ? Is it true that react js supports SEO support
clean up in useEffect
What is the use of useCallback and useMemo
Why do we need keys in react less
Do you know about redux




## High Order Component in react js ?

HOC is a method of reusing the component functionality logic. 
It simply takes the original component and returns the enhanced component.

Reason to use Higher-Order component:

--Easy to handle
--Get rid of copying the same logic in every component
--Makes code more readable



## Do you know about SEO ? Is it true that react js supports SEO support - yes

While React is often lauded for making front-end development more efficient, this popular library can be problematic for search engines if we do not set up the website properly.
Search engine optimization (SEO) is the process of improving the ranking (visibility) of a website in search engines.
The higher (or more frequently) a website is displayed in a search engine list (like Google), the more visitors it is expected to receive.
SEO considers how search engines work, what people search for, and which search terms (words) are typed.
Optimizing a website may involve editing the content to increase its relevance to specific keywords.
Search engine optimisation (SEO) is the process of improving the quality and quantity of website traffic to a website or a web page from search engines. SEO targets unpaid traffic (known as “natural” or “organic” results) rather than direct traffic or paid traffic.
React helps build a very user-friendly UI that is also valuable by SEO, so you definitely shouldn't avoid it while creating a user interface for your app/website. However, you should use some tricks to ensure that your React-site is understandable for Google crawlers and, therefore, good for SEO.



## clean up in useEffect

useEffect Hook is to eliminate the side-effects of using class-based components.

For example, tasks like updating the DOM, fetching data from API end-points, setting up subscriptions or timers, etc can be lead to unwarranted side-effects.

clean up function: this function gets executed when the component is unmounted from the screen. This is mostly used for memory leaks. //componentWillUnmount : Cleanup function in useEffect. useEffect(() =>{ console.log("Inside useEffect hook");

return function cleanup() { console.log("componentWillUnmount is happen...!") } })
 

## What is the use of useCallback and useMemo

The useCallback hook is used when you have a component in which the child is rerendering again and again without need.

Pass an inline callback and an array of dependencies.

useCallback will return a memorized version of the callback that only changes if one of the dependencies has changed.

prevent unnecessary renders.

const memoizedCallback = useCallback( () => { doSomething(a, b); }, [a, b], );

return memorized function

This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders.



The useMemo is a hook used in the functional component of react that returns a memoized value. memoization is a concept used in general when we don’t need to recompute the function with a given argument for the next time as it returns the cached result. A memoized function remembers the results of output for a given set of inputs.

ex:- 1+2=3 ,whn we enter same input again it give catched value without doing the addition

The useMemo hook is used to improve performance in our React application.

returns a memoized value.

React has a built-in hook called useMemo that allows you to memoize expensive functions so that you can avoid calling them on every render. You simple pass in a function and an array of inputs and useMemo will only recompute the memoized value when one of the inputs has changed.


## Do you know about redux

Redux is a pattern and library for managing and updating application state, using events called "actions". It serves as a centralized store for state that needs to be used across your entire application, with rules ensuring that the state can only be updated in a predictable fashion. Here is a small example of react and Redux application. You can also try developing small apps. Sample code for increase or decrease counter is given below - This is the root file which is responsible for the creation of store and rendering our react app component. /src/index.

Redux is a predictable state container designed to help you write JavaScript apps that behave consistently across client, server, and native environments and are easy to test. While it's mostly used as a state management tool with React, we can use it with any other JavaScript framework or library.

Store, Reducer, Action, Dispatch

Redux is a predictable state container for JavaScript apps.

The most common use case for Redux  is for communicating asynchronously with an external API to retrieve or save data. Redux makes it easy to dispatch actions that follow the lifecycle of a request to an external API. Redux is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises.

One of the main use cases for this middleware is for handling actions that might not be synchronous, for example, using axios to send a GET request.