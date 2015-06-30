title:                  Seeing Stars: Building Variable Rating Component 
description:             
duration:               2 hours  
skill_level:            Intermediate  
core_concepts:          [To come]
prerequisite_concepts:  [To come]  

tags:                   React  
date_implemented:       June 30, 2015  
slug:                   seeing-stars-react 

You've been hired by Netflix to spice up their website with a new stars rating view in React. Some movies, they tell you, are going to have a bonus _sixth_ star in addition to the original five, which they figure will really up their average ratings. If that goes well, a seventh star might even be on the event horizon.

To future-proof your system, you decide to make a react component that takes `n` stars and shows the rating on it from 0 to `n`.

## Milestone 1
- Write a React component that takes in a value from 0 to 1 and shows a bar with that ratio of the width colored in yellow, beginning from the left edge. It should look like a progress bar (0 is empty, 1 is full).
- Add a star-shaped clipping mask to your component in so it looks like a star. It's a star, you're a star, we're all stars here. 
- Hint: [This clippy](http://bennettfeely.com/clippy/) might come in handy, but [this clippy](http://www.tuckertechtalk.com/wp-content/uploads/2015/01/clippy_paper.jpg) probably won't.

## Milestone 2 - Putting your stars in alignment
- Write a React that takes in a `max` and a `rating` and displays `max` stars with `rating` of them filled in. stars should "fill up" from left to right, with the last star (if the `rating` is < `max`) only partially filled.
- Set some reasonable defaults for your `props` so that your component works without having to pass anything into it

## Milestone 3
Netflix has decided to switch up their styleguide and now all the stars need to be green with purple backgrounds. Moreover, now they want the rating system to be made out of circles instead of stars as a reference to their roots in DVDs. More changes are bound to come your way, so you decide to make the component as flexible as you can.
- Define some `props` that apply styles to your react components for color, size and clipping mask, as well as some other fun properties. Add some default `props` for those too.
- Create a demo that renders a few components in different colors, shapes and sizes.
- Give yourself five stars (or seven)!

[Example solution here](http://codepen.io/ripleyaffect/pen/WvXvEo)
