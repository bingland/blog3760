---
title: "Todo App Reflection"
date: 2020-09-27T17:39:09-06:00
draft: false
---
![Todo App Screenshot](/images/todolist.png)

My JavaScript file had two main functions that would be called everytime I wanted to update my todos or any time I wanted to update the categories listed. The HTML document had almost no content besides an h1, I inject everything aelsell in there via JavaScript. I also had some other functions that I didn't need to put in these two main functions, such as functions that readjust all the id's, one that keeps the todos / categories in sync with the localStorage, and others.

I was trying to think of my application almost like a React application; where you have a state, and everytime the state is changed, the todo and category "components" update by running the two main todo and category functions. There are definitely better ways I could have done this, especially in terms of organization. 

As I said before, my app got a little bit messy at some points. One problem was that my renderTodos and renderCategories functions were pretty big. The reason for this was because I added all of my event listeners in there, as well as some other random stuff. I think I could have organized my app better; maybe instead of just having two big renderTodos and renderCategories functions, I could have just not rendered a list of categories / todos everytime something changes, and just add a Todo only when it's added, add the event listeners once, delete it once, and so on. This way I could have organized everything a bit better into their respective functions. 

I also had some other issues with how I was giving todo's their ID. What I did was I'd have the ID of a new todo equal the length of the initialTodos array, and I would also remove elements via their id as well. However, this makes things a little complicated because whenever I would delete a todo in the beginning or the middle of my todos, I'd have to readjust them all. So what I did to solve this was to add a data-id attribute, like Landon did in our lectures, as well as getting the index of an item using findIndex() and getAttribute(). Also, to make matters worse, I accidentally used for of loop instead of a for in loop, and it took me a while to figure that out for some reason. 