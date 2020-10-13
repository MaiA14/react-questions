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
10) **What is a higher order component**\
      A higher-order component (HOC) is an advanced technique in React for reusing component logic. 
      They are a pattern that emerges from React's compositional nature. 
      Concretely, a higher-order component is a function that takes a component and returns a new component.
11)  **What is Redux**\
       the entire application state is kept in a single store. The store is simply a javascript object. 
       The only way to change the state is by firing actions from your application and then writing reducers for these actions that modify the state. 
       The entire state transition is kept inside reducers and should not have any side-effects.
       Redux is based on the idea that there should be only a single source of truth.
12) **What is Redux Thunk used for?**\
      Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, 
      or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.
13)  **What is PureComponent? When to use PureComponent over Component?**\
       You should use it when a component could re-render even if it had the same props and state. An example of this is when a parent component had to re-render but the
       child component props and state didn't change. The child component could benefit from PureComponent because it really didn't need to re-render.
14)  **How Virtual-DOM is more efficient than Dirty checking?**\
       The virtual DOM is used for efficient re-rendering of the DOM. This isn't really related to dirty checking your data. ... In fact, the diff algorithm is a dirty
       checker itself but it is used to see if the DOM is dirty instead. We aim to re-render the virtual tree only when the state changes.
15)  **Is setState() is async? Why is setState() in React Async instead of Sync?**\
      This is because setState alters the state and causes rerendering. This can be an expensive operation and making it synchronous might leave the browser unresponsive.
      Thus the setState calls are asynchronous as well as batched for better UI experience and performance.
 16)  **What is render() in React? And explain its purpose?**\
      The ReactDOM. render() function takes two arguments, HTML code and an HTML element. The purpose of the function is to display the specified HTML code
      inside the specified HTML element.
17)  **Explain the components of Redux?**\
      - Action — Actions are payloads of information that send data from our application to our store. They are the only source of information for the store. 
        We send them to the store using store.dispatch(). Primarly, they are just an object describes what happened in our app.
      - Reducer — Reducers specify how the application’s state changes in response to actions sent to the store. 
        Remember that actions only describe what happened,
        but don’t describe how the application’s state changes. So this place determines how state will change to an action.
      - Store — The Store is the object that brings Action and Reducer together. The store has the following responsibilities: Holds application state; Allows access to state
        via getState(); Allows state to be updated via dispatch(action); Registers listeners via subscribe(listener); Handles unregistering of listeners via the function
        returned by subscribe(listener).
18)  **What is React.cloneElement? And the difference with this.props.children?**\
      React.cloneElement clone and return a new React element using using the passed element as the starting point. The resulting element will have the original element's
      props with the new props merged in shallowly. New children will replace existing children. key and ref from the original element will be preserved.
      React.cloneElement only works if our child is a single React element. For almost everything {this.props.children} is the better solution. 
19)  **What is the second argument that can optionally be passed to setState and what is its purpose?**\
       A callback function which will be invoked when setState has finished and the component is re-rendered.
20)  **What is the difference between React Native and React?**\
       React Native is an entire platform allowing you to build native, cross-platform mobile apps, and React. js is a JavaScript library you use for constructing a high
       performing UI layer. ... Like the browser code in React is rendered through Virtual DOM while React Native uses Native API's to render components on mobile
       
       
       Sources: https://medium.com/@vigowebs/frequently-asked-react-js-interview-questions-and-answers-36f3dd99f486


