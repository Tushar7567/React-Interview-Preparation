## What is Virtual DOM?

Virtual DOM is representation of JS DOM
It is similar to real DOM but it cannot directly change the real dom.
React maintains 2 virtual dom
Whenever there a change in document, it compares previous state of virtual dom with the updated state of virtual dom and this comparision is called Diffing Algorithm.
It sends the changes to real dom in the form of batch 
It makes react fast.(at the time of comparision, it translate the code)
So this whole process is called reconcilation(comparision and applying the changes to real dom).

## What is SPA

It dynamically re-renders the webpage with a new data from web-server
Browser re-renders the content without reloading the website
![image](https://learn.microsoft.com/en-us/archive/msdn-magazine/2013/november/images/dn463786.wasson_figure2_hires(en-us,msdn.10).png)


## What is difference between class and functional component

### class component
Class components can be used when you are doing data operations and server calls.
Contain lifecycle methods
Constructor structure is required since these are class components.
Contains state variables.

### functional component
Functional Components can be used mostly when you want to create dumb or stateless components  
These components does not have lifecycle methods, they have hooks like useEffect
Complete constructor structure is not required in these components, so they are easy to handle
Do not have state variables, they have hooks like useState


## What do you mean by state and its use in react?

States are variables which are used to manipulate data
States are muttable
Any changes in these variables force react to re-render the DOM and update the components


## What is JSX and why do we use it instead of js?

JS XML
It allows us to write HTML in react
JSX is faster than js because it performs optimization of code while translating to regular js(by Babel).
It is easier to manage and debug easily.

In JSX,
we have to return one element
all self closing tags should be closed
we cannot use js reserved keywords (like class---className, for--HTMLfor)

## Package.json

It is the heart of any Node project.
It records important metadata of the project 
All data is stored in a json format
It contains all dependencies, and properties of project
npm init--is used to create a package.json file
