---
title: "Functions, Callbacks and Promises"
date: 2021-03-06T18:20:47-07:00
draft: false
---

### Functions

**How to declare a function. (3 ways)**

```javascript
function example () {
    // function code here...    
}

const example = () => {
    // function code here...
}

const example = function () {
    // function code here...
}
```

**How to return a value from a function**

```javascript
function example () {
    return 'returning a cool string'
}
```

**How to accept a value into a function**

```javascript
const add = (a, b) => {
    return a + b
}
```

### Callbacks

**What is a callback? How do they work?**

Callbacks are in a nutshell code that runs after a section of code has finished. Callbacks are typically functions that can be passed as an argument into another function, and then be executed later. 

**When might you use one in your own code?**

You might want to use a promise in a situation where you want to execute some code after some other code as finished executing. A great situation to use a callback would be with a promise. You typically use promises when you're making an API request, so after a promise resolves is a great time to do a callback. 

### Promises

**What is a promise? How do they work?**

Promises are objects that may produce a value in the future. Either a promise will eventually resolve or not. A promise can be in three states; fulfilled, rejected, or pending. You can attach callbacks to promises so that when they fulfill, you can handle the data it sends back as you'd like.

**When might you use on in your code? (Provide an example not using a built in method such as fetch())**

You can use promises whenever you need to perform an asynchronous function, or many asynchronous functions of course. One specific example of this might be writing / reading a file that takes a bit of time to complete. 

**What is the async, await syntax? How does it work?**

Here's an example of the the async await syntax:

```javascript
const example = async () => {
    let promise = await fetch('http://example.com/movies.json')
    let data = await promise.json()
    return data
}
```

In this example, using the async keyword when you declare the function allows you to use the await keyword. Await does exactly what it sounds like; it waits for the promise to either resolve or reject before assigning a value. 

**Why is the async, await syntax helpful?**

In my example, if you didn't use the async / await syntax, then the function would just return data as a pending promise. However, using the await keyword, it waits for the promise to resolve and returns a resolve or rejected promise. You can use async / await in any situation where you need to wait for a value to be assigned before doing something with that variable. 
