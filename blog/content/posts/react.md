---
title: "React Blog Post"
date: 2021-03-20T20:27:02-06:00
draft: false
---

**What is React? Who developed it and for what reason?**

React is a JavaScript library created by Facebook used for building reactive, component based applications. Even though React is technically a library, many people would also call it a "front-end framework" along with Vue and Angular. 

React was developed to greatly improve the application development process. If you write an application in vanilla Javascript, you may find yourself having to jump through hoops to get your code to update, divided into components, and so on; but React makes this extremely simple. React shines when your data changes over time, and renders changes on the fly. It's also great for breaking your code into components.

**What is state?**

The state is where you can store values and functions that belong to a component, or to the entire application itself. 

**What is the difference between a functional component and a class component? When should you use each type?**

Functional and class based components are both components that render JSX, however class based components are extended by the React.Component library, whereas a functional component is just a regular Javascript function. Another difference between functional and class based components is how props are passed down. Another difference between them is state and lifecycle methods. In the past, only class components could handle state and lifecycle methods, however as of React 16.8, React hooks can be used for state and lifecycle methods. 

In terms of when you should use each type, I personally think that functional components are better because they're easier to read, write and debug, and also have less code than class based components. However, since React hooks are new compared to class based components, many old projects may already be running on class based components. In the end I think I would say that it just comes down to personal taste, although hooks and function based components seem a bit more popular.

**What is JSX?**

At it's core, JSX is basically just JavaScript, although it looks like it's a combination of Javascript and HTML. The browser obviously doesn't stand JSX since it's not valid JS code, so React uses Babel to convert JSX to JavaScript. All JSX elements are converted to the React.createElement function. 

**What does it mean to 'lift state up'?**

Lifting state up in React just refers to lifting shared state up so that two components with a shared parent can share information between eachother. If there are two components that need to share state, then usually the best approach is to move the shared state up to a common parent. 
