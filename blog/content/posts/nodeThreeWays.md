---
title: "Node 3 Ways Post"
date: 2020-10-11T22:38:16-06:00
draft: false
---

Node JS is a Javascript runtime built on Chrome's V8 JavaScript engine. It is event-driven and asynchronous. It's also often described as back-end JavaScript, or JavaScript run outside of the browser, on a server or on your own computer. You can use Node JS for a ton of things, such as: 

**Scalable applications -** Node JS is a fantastic choice when it comes to applications that aren't CPU intensive. It's able to handle large amounts of request, whether it's big or small. It's why a lot of companies choose it for their backend. 

**Rest API's -** Rest API's are pretty much always not CPU intensive, which naturally makes them a perfect fit for Node. Node is great at handling HTTP requests, which is perfect for Rest API's. 

**Real time applications -** Since Node JS is asynchronous and event-driven, it's very easy to make fast and high performance real time applications, and it's great for handling high traffic. 

**Chat applications -** Chat applications fit into real time applications; it's one example of them. It's extremely easy to deliver messages to other users in real time with Node. 

Node JS differs from regular JS in the browser in many different ways. Node JS doesn't have any access to any kind of DOM manipulation, because there isn't a DOM to manipulate. That means there's no such thing as document.querySelector() or anything like that. However, with Node being a Javascript runtime, you have access to many new kinds of functions and modules, such as being able to read and write files, create servers, get and send requests, and so on.

Express JS is a framework for Node JS designed for making the HTTP module much more minimalistic and easy to use. Express JS is useful because it helps you organize your web application into an MVC architecture on the server side, makes setting up a server with the HTTP module a lot easier, and just provides a thin layer of features without veering too far off from what Node JS is all about. 

Template engines are useful for turning static files into functional webpages via variables. I was at first confused as to why anybody would ever consider using a template engine when front end frameworks like React and Vue exist, but template engines are "logicless" a lot more lightweight compared to a frontend framework. Or at least that's what it seemed like to me. I decided to go with express-handlebars because the syntax is really easy to understand and you don't have to change the syntax of the HTML file, you just need to add brackets like Vue does. 