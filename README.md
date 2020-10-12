# react-questions

1) **How React works? How Virtual-DOM works in React?**\
   React uses virtual DOM to enhance its performance. It uses the observable to detect state and prop changes. 
   React uses an efficient diff algorithm to compare the versions of virtual DOM. 
   It then makes sure that batched updates are sent to the real DOM for repainting or re-rendering of the UI.
2) **What is JSX?**\
   JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.
3) **What is React.createClass?**\
   React. createClass allows you to generate component "classes." 
   Under the hood, your component class is using a bespoke class system implemented by React.
   With ES6, React allows you to implement component classes that use ES6 JavaScript classes. The end result is the same -- you have a component class.
4) **What is JSX?**\
   JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React.
5) **What is React.createClass?**\
   React. createClass allows you to generate component "classes." 
   Under the hood, your component class is using a bespoke class system implemented by React.
   With ES6, React allows you to implement component classes that use ES6 JavaScript classes. The end result is the same -- you have a component class.
6) **What is ReactDOM and what is the difference between ReactDOM and React?**\
   Without react-dom . The ReactDOM module exposes DOM-specific methods, while React has the core tools intended to be shared by React on different platforms (e.g. React Native). 
   To be more concise, react is for the components and react-dom is for rendering the components in the DOM.
7) **What are the differences between a class component and functional component?**\
   The most obvious one difference is the syntax. A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element. 
   A class component requires you to extend from React. Component and create a render function which returns a React element.
8) **What is the difference between state and props?**\
   The state is a data structure that starts with a default value when a Component mounts. It may be mutated across time, mostly as a result of user events.
   Props (short for properties) are a Component’s configuration. Props are how components talk to each other.
   They are received from above component and immutable as far as the Component receiving them is concerned.
   A Component cannot change its props, but it is responsible for putting together the props of its child Components.
   Props do not have to just be data — callback functions may be passed in as props
9) **What are controlled components?**\ 
   - A Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. 
     A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. 
     You could also call this a "dumb component"
   - A Uncontrolled Component is one that stores its own state internally, and you query the DOM using a ref to find its current value when you need it. 
     This is a bit more like traditional HTML.
10) **What is a higher order component?**\  
      A higher-order component (HOC) is an advanced technique in React for reusing component logic. 
      They are a pattern that emerges from React's compositional nature. 
      Concretely, a higher-order component is a function that takes a component and returns a new component.
11) **What is Redux?**\  
       the entire application state is kept in a single store. The store is simply a javascript object. 
       The only way to change the state is by firing actions from your application and then writing reducers for these actions that modify the state. 
       The entire state transition is kept inside reducers and should not have any side-effects.
       Redux is based on the idea that there should be only a single source of truth
