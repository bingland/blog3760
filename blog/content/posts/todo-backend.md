---
title: "Todo Backend"
date: 2020-10-28T23:36:17-06:00
draft: false
---

My application is only running on Heroku, of course with NodeJS as the backend. I have one main.js file that contains all the server logic and is written with Express, and I use my SRC folder as the static folder, where when you visit the root of the site, it serves you index.html with all the CSS and JavaScript attached to it as well. When I programmed the todo app, I made tried to mimic React in a way; meaning that everytime the "state" updates, I have to main renderControls() and renderTodos() functions that render everything. I made GET, POST, PUT and DELETE endpoints that could be reached at /todos, and my frontend was able to make fetch requests to that and make todos, delete them, modify them, and so on. I also made it so that when I make a change to the database, it sends me back a list of all of the todos, and I update my entire application based off of that. If for some reason a PUT request or something like that doesn't work out, then the list of todos on my site won't be different from what's on the database.

I decided to just put everything on Heroku because it seemed simpler to just have everything in one spot. If I was making a todo app outside of class, like for a company or something, it wouldn't make much sense to have the front end on one server and the backend on a different one. At least that's what I think, maybe there are situations where this could be different.

Modelling the data for the todos on the database was pretty simple using MongoDB, basically I just had a todo database, where each todo has its own text, category, and completed properties. And of course the ID attribute just automatically gets tagged on by MongoDB, which is really nice. 

Documentation is very important when it comes to collaborating with other people, when other people are going to going to be using / viewing your code, or when you're going to be using / viewing somebody elses code. Adam and I are together in a group for the Interaction Design Practicum, where we're basically fixing a bunch of problems with somebody's site. When we started working on the project, we just had no clue whatsoever on how the site was even working, so we had to do some serious detective work to get through the mess that the site is. Let's just say that the sites backend is written in PHP :)