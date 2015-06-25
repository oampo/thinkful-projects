title:                  Hello KnoBe: First Node Server  
description:            Write your first Node server that returns different content depending on the URL.  
duration:               2 hours  
skill_level:            Beginner  
core_concepts:          Node, servers, Express, request parameters, string concatenation, array slicing  
prerequisite_concepts:  Proficiency with JavaScript  

tags:                   Node  
date_implemented:       June 23, 2015  
slug:                   jedi  


## Project Brief

Create a server which, when a user visits the /jedi URL, should work out the user's Jedi name and greet them. Your Jedi name is the first three letters of your last name, followed by the first two letters of your first name. So visiting /jedi/Beyonce/Knowles should respond with "Hello KnoBe".

##Milestones

### Milestone 1: Get your server running

- Create a server which returns "Hello World" when you visit the root URL `/`.
- Next, add a route to your server to handle the first and last name from the URL in the form `/jedi/:firstname/:lastname`. To make sure you're requesting data from the URL correctly log the first and last names to the console. Move on the the next milestone once you're logging the full names to the console. If you need help with either step, review [Simple Express servers and Request parameters](https://courses.thinkful.com/node-001v4/assignment/2.1.1). 

### Milestone 2: Greet the Jedi

1. Now that your server is getting the first and last names, combine them into a single string. 
Here's a refresher on [string concatenation with JavaScript](https://courses.thinkful.com/node-001v4/assignment/1.1.2).
2. Next, slice the name string to just the first three letters of the last name and the first two letters of the first name (hint: you may want to use [array slicing](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/slice). 
3. Finally, return the Jedi name to the browser. If you need help, review this lesson on [returning JSON from a Node server](https://courses.thinkful.com/node-001v4/assignment/2.2.2).

## Example Solution

Once you've tried the project on your own take a look at the [sample solution here.](https://gist.github.com/oampo/41eec381254a01462bdd#file-jedi-js)
