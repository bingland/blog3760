---
title: "Final Post 6"
date: 2020-12-13T23:37:10-07:00
draft: false
---

**What have you done this week?**

This week I was able to add a submit review area to a dishes page. When you click on the new review button, it opens up a new area where you can type in a review title, the body, and add a rating. For that rating, I made it so you can interactively click a star and it will update when you click it. When you click the cancel button, the review area collapses and reverts back to just showing the new review button. I was also able to connect this to the backend; so when you click the submit button, it sends a POST request to my server and adds the review to the database.

**What do you plan on doing next week?**

When you add a review to the database, it needs to have some kind of confirmation message to show that the review was successfully submitted. I also need to add in some sort of form check to make sure that the user isn't submitting with any empty fields, or even check if they're injecting code or using strange characters. I have no idea if you can inject code this way on MongoDB but I do know that this kind of security vulnerability can occur with SQL and is called SQL injecting. Aside from this, I would also like to add the ability to add completely new dishes or restaurants to the database. This is important because if a user visits a restaurant that isn't very popular, they may want to add a dish / restaurant that doesn't exist yet. I would also like to explore the possiblity of searching for restaurants on a map using some kind of API. 

**What roadblocks did you encounter and what did you do to overcome them?**

This week it was a little bit of a struggle to add, remove, re-add and re-remove elements from the DOM. In React this is pretty straightforward, but in vanilla JS, you have to make pre-written DOM elements, and then insert that into the DOM. Hopefully that makes sense. Before I would just use .innerHTML for everything but in my case it didn't quite pan out. I also was a bit low on time this week so I didn't quite finish everything that I would have liked to finish this week, but after tomorrow morning this should be the only final project I have left, so I'll be able to focus on it until Thursday night. 