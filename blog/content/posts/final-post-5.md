---
title: "Final Post 5"
date: 2020-12-06T23:39:15-07:00
draft: false
---

**What have you done this week?**

This week I did a bunch of things with my project. I added some more meta data for restaurants and also for dishes. My restaurants now have menu, drivethru and delivery values, and my dishes now have a thumbnail and tags. I added tags so that now I can search by the dish tags and not just their name. This is useful because now if I search "taco", it'll pull up tacos and not just stuff with "tacos" in its name. I also was able to hook up all this backend info to the frontend. I also added the functionality to add a review via a POST request. I was working on hooking that up to the front end today but was writing sloppy code so I haven't quite finished and comitted that yet. 

**What do you plan on doing next week?**

Next week I want to finish the functionality to add a review for a dish via a POST request on the frontend. I almost have this finished though. I also want to add the ability to edit reviews and delete them. After that point I'd like to be able to edit, add and delete information for restaurants and dishes. I think adding these as server endpoints will be easy but it'll maybe be a little bit tricky to implement into my frontend. I would also like to explore searching for restaurants on a map, using the Google Maps API or a Bing Maps API or something like that, whichever's better. After this I think I will probably start making my site look pretty. I have basic SCSS implemented now but it doesn't look polished. 


**What roadblocks did you encounter and what did you do to overcome them?**

Most of the challenges that I ran into relate to the Node server / Mongoose. The first tricky hurdle that I overcame was using an $or query for mongoose. The second one was updating ObjectIDs that are connected to other templates. For example, I would create a new dish, but it wouldn't show up when I called restaurants; so I had to find the restaurant after adding the dish, and then adding the dish ObjectID into it. I used .findOneAndUpdate() for this, as well as a $push query, if that's what it's called. Also, as I mentioned before, I was writing messy code when I was adding the functionality to add a review via a POST request, so I don't have that quite finished. 