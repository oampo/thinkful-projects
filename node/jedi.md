Level: Beginner

Time: 2 hours

Goals: Write your first Node server that returns different content depending on the URL

Concepts: Node, servers, Express, request parameters, string concatenation, array slicing

Pre-reqs: Proficient with JavaScript

## Project

Create a server which, when you visit the /jedi URL, should work out what a person's Jedi name is and greet them. Your Jedi name is the first three letters of your last name, followed by the first two letters of your first name. So visiting /jedi/Beyonce/Knowles should respond with "Hello KnoBe".

## Steps

Milestone 1: Get your server running

1. First, create a server which returns "Hello World" when you visit the root URL.
2. Next, request the first and last name from the URL in the form `/jedi/:firstname/:lastname`. To make sure it's working log the names to the console. When you see the first and last named logged to the console, move on to the next milestone. 
If you need help with either step, review [Simple Express servers and Request parameters](https://courses.thinkful.com/node-001v4/assignment/2.1.1). 

Milestone 2: Greet the Jedi

1. Now that you're requesting data from the URL to the server, concatenate the string into one name. If you need a refresher on concatenating with JavaScript, you can find one [here](https://courses.thinkful.com/node-001v4/assignment/1.1.2).
2. Next, slice the string to just the first three letters of the given last name and the first to letters of the first name (hint: you may want to use [array slicing](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/slice). 
3. Finally, return the Jedi name to the browser. If you need help, review this lesson on [returning JSON from a Node server](https://courses.thinkful.com/node-001v4/assignment/2.2.2). 
