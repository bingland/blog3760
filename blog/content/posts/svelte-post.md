---
title: "Svelte Post"
date: 2021-02-23T12:07:33-07:00
draft: false
---

I didn't realize that React was inefficient. It doesn't doesn't have any sense of the values in the code, it can't tell what's reactive and will just run code repeatedly. They use things such as useMemo, useCallBack, shouldComponentUdate and so on to tell React what code doesn't need to be run repeatedly, and this is a symptom of it being underpowered. 

One thing that I like about Svelte is how simple it is to do things that are more complicated in React. For example, if you want to update the state, all you need to do is just... _update_ it. No "this.setState()" required or anything, you can just change the state like you would a normal variable in JavaScript. React components also tend to be 40% larger than Svelte components. 

Another interesting thing brought up in the presentation is how Svelte is being used in the embedded web for many smaller devices. Companies that don't want to worry so much about performance (maybe do to a lower level of specs on their hardware) are using Svelte for their products. In my mind, embedded web apps haven't always been great because I've had bad experiences with them, but this was many many years ago; so it's very interesting that this is becoming a thing again in some places. 

