---
title: "Final Post 2"
date: 2020-11-15T21:35:09-07:00
draft: false
---

**What have you done this week?**

This week I mainly worked on the frontend for my site. Right now I only have GET requests on my server ready, but I've decided to focus on the front end first because I want to make sure I know exactly what attributes and properties I want for my models. I actually have only one dish, one restaurant, one user and one review at the moment because it'll be a pain in the butt to add one attribute to 50 reviews, for example. This week I added a calorie attribute to my dish and also added images to the dishes, as well as for the user profile picture. For the record, I'm not actually storing images at the moment, I'm just copying an image link from a different site. I also added basic SCSS to the site; it doesn't look amazing at the moment but it's just for the overall structure, as the final design of my site is still up in the air. In terms of JS, I have it so all the dishes for my site list out when I search for a dish, and when you click on one, it displays all of its information such as reviews, what restaurant it belongs to, all of its photos, and other meta deta. Next week I will work on this more.

**What do you plan on doing next week?**

As I mentioned in the paragraph above, I want to make it so all the metadata for a dish displays when I click on a dish. I also want to decide what metadata I'm displaying exactly. I think there's data that I could display about the restaurant that the dish belongs to, such as it's other popular dishes, what times the restaurant opens and closes, if the restaurant does takeout or not, and so on. It would also be ideal to have a seperate page to view all the restaurants dishes, and which ones are the highest rated. After I do this, I'd like to be able to add dishes via POST requests; however this is going to take a bit of time because when you add a dish you also have to attach which restaurant it belongs to, images, and so on. That is still a little bit of a gray area for me, but I think as I work on this project, the picture will become clearer naturally. 

**What roadblocks did you encounter and what did you do to overcome them?**

I don't think that I really encountered any big roadblocks this week. I mainly just thought about what ways are the best for me to optimize my app, as well as my database structure. One thing that I discovered which I thought was useful was that I can generate arrays using map and foreach and all that stuff in a template literal using ${}. Maybe this is a small thing, but I think my react class taught me this and it's nice to know that I can do the same thing in vanilla JS. 