---
title: "Final Post 3"
date: 2020-11-22T20:30:02-07:00
draft: false
---

**What have you done this week?**

This week I started to list out the user reviews for a dish when you select that dish, along with some SCSS styling for that. I also made it so that for the dish rating it displays as stars and not as a number. So for example, a value of 4.5 would display 4 full star SVG's and one half star SVG. I also made a function that converts the Date object for a review into something a human can read. Some more things that I did this week was add another dish to my database, added the functionality to GET dishes by query, connected that to the front end search box that I had set up previously, added the functionality to GET restaurants, and output the dishes for a restaurant on the frontend for when you select a dish. I had a little problem with outputting the dishes though, I'll explain that in more detail in the roadblocks section.

**What do you plan on doing next week?**

For the server, I would like to add the functionality to GET a restaurant by it's ID or name, and start working on the ability to POST reviews to my database. I would also like to finish outputting the dishes for a restaurant when you select a dish, as well as add some more properties to each restaurant in my database; such as if the restaurant does takeout or not, when its open, their website, and so on. I would also like to make my search feature a little bit better. Right now my server will decide whether or not to return a dish based off of it's name only. So for example, if you search for tacos, you won't get any results; but if you search for "Cheesy Gordita Crunch", then you'll get that taco. So in order to combat this I think I will have to add "tags" to each dish, or maybe even a category. 

**What roadblocks did you encounter and what did you do to overcome them?**

One of the roadblocks that I encoutered was that I accidentally didn't make a property in one of my models an Array, so I was really confused as to why my restaurants were only displaying one dish. I checked the models and didn't see the typo at first; but then I checked back later and realized what the problem was. Another problem that I had was when I was trying to display the dishes of a restaurant for the selected dish via fetch / promises was that when I was outputting the values to the DOM it would display as [object Promise]. I didn't solve this bug this week but I am pretty sure I know why it's doing that. I think I am displaying the content to the page before the promise resolves, so I need to change how my code is layed out a bit better so that the promise resolves first, and then outputs that data to the DOM. 