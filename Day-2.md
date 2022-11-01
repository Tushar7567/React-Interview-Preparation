## What is the Difference between react and react native? Which one is library or framework?

ReactJS:-
It is a JavaScript library that supports both front-end and server-side.
It is a popularly used library, which focuses on developing user interfaces (UI) for mobile as well as web-based applications.
Developed by Facebook
it is based on the JavaScript language and hence, it is synonymously also called ReactJS
Virtual DOM is used
command for creating React JS -> npx create-react-app react-demo
cd react-demo
npm start
Facebook,Netflix,Medium

React Native:-
React Native is a cross-platform mobile framework that uses the ReactJS framework
As the name suggests, it is primarily used for developing “native” mobile applications (like Windows, iOS as well as Android).
Also developed by Facebook

The major advantage provided by React Native is that it allows the developers to create mobile applications on various different platforms without compromising the end user’s experience.



## What is the package name you are using for routing

React Router, React Router DOM
React Router is a standard library for routing in React.
React Router is the most popular library for implementing routing for React apps.
It enables the navigation among views of various components in a React Application,
Allows changing the browser URL, and keeps the UI in sync with the URL.
A tool that allows you to handle routes in a web app, using dynamic routing. Dynamic routing takes place as the app is rendering on your machine
It provides the synchronous URL on the browser with data that will be displayed on the web page.
A that keeps the history of your “URL” in memory
Router is mainly used for SPA It has a simple API with powerful features like lazy loading,dynamic route matching,and location transition handling.


## How do you pass data from parent to child

Props: It allows you to pass data from a parent component to a child component.
Stands for properties.
Props are basically kind of global variable or object.
We can access any props inside from the component’s class to which the props is passed.
The props can be accessed by:- this.props.propName



## What is lazy loading in react ?

Lazy loading (also called on-demand loading)
It is an optimization technique for the online content, be it a website or a web app.
Instead of loading the entire web page and rendering it to the user in one go as in bulk loading, only the required section and delays the remaining, until it is needed by the user.
One form of lazy loading is infinity scroll, in which, the content of the web page is loaded as and when the user scrolls down the page. It is a popular technique being used by various websites.
On-demand loading reduces time consumption and memory usage thereby optimizing content delivery.
Unnecessary code execution is avoided.
Optimal usage of time and space resources makes it a cost-effective approach from the point of view of business persons.


## Difference b/w Stateful and stateless Component

In React, a stateful component is a component that holds some state.

A stateful component is always a class component. It is created by extending the React.

stateful components can have stateless components inside them, while the stateless components are a plain JavaScript function.

Stateless components, by contrast, have no state.

Stateless components are those components which don't have any state at all, which means you can't use this. setState inside these components.

It is like a normal function with no render method. It has no lifecycle, so it is not possible to use lifecycle methods such as componentDidMount and other hooks.

Note that both types of components can use props. In the example, there are two React components.

## How do you switch one component to another, Conditional Rendering

React Router

Link

NavLink

Using conditions with logical && operator

Conditional Rendering:- ! Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them. ! That is to create multiple components and render them based on some conditions. This is also a kind of encapsulation supported by React.

