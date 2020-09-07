---
title: "Functions, Objects, Arrays"
date: 2020-09-06T19:12:42-06:00
draft: false
---

**What are functions in Javascript?**

Functions are a block of reusable code that can be used to execute the code inside of it.

Callback functions are functions that are passed into another funciton as an argument, and are called inside of the function.

A promise is an object that may or may not produce a value over a certain amount of time. It may resolve, it may not resolve. When a promise resolves, it typically fulfilled an action or value. 

**What are objects in Javascript**

Objects are used to store data, and give properties and fuctinoality to variables. In object oriented programming, they have a pretty wide definition, because they can be anything that stores data. However, in this context, they contain many values and properties. You can define an object in many different ways, but here's an example:
```javascript
let phone = {brand: 'Apple', os: 'iOS', color: 'silver', price: '1000', inStock: true}
```
One way to loop through an object is with a for...in loop:
```javascript
const object = { a: 1, b: 2, c: 3 };

for (const property in object) {
    console.log(property)
}
```

**What are Arrays in Javascript?**

Arrays are data structures that are collections of elements. You can put as many elements as you want in it, it's like a list. They are defined using square brackets. 

There are a ton of ways to loop through arrays. One way is to use a for..in loop :
```javascript
const list = ['carrots', 'watermelon', 'meat', 'eggs'];

for (let i in list) {
    console.log(i)
}
```
You can also use forEach:
```javascript
const list = ['carrots', 'watermelon', 'meat', 'eggs'];

list.forEach(item => {
    console.log(item)
})
```

**Write about at least one other thing you learned this week.**

One thing that I learned that was pretty useful, was using Object.entries() to display the key and value of an object. Here's what I did for a problem on one of our recent assignment: 
```javascript
export const objToArray = ( obj ) => {
    let results = []
    for (let [key, value] of Object.entries(obj)) {
        results.push([key, value])
    }
    return results
};
```