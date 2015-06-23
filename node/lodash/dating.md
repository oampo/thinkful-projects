title: Functional Programming with Lodash
description: Use some of the most common Lodash methods to solve complex problems with simple code.
duration: 4 hours
date_implemented: 
skill_level: Intermediate
slug:
tags: Node

Concepts: Functional styled JavaScript; Data management of Collections and Objects; Partial Application, Composition and Combinators

## Project Brief

These days, lonely coders rely on online learning to get to know new languages. But let’s be honest: one-app stands with the wrong language can lead to recurring bugs. Gone are the days of swiping left and right for the next best thing. Programmers are looking for languages they can trust.

You’re the lead developer for Java Meets Bagel, a service that takes a user’s personal interests and matches them with courses that help them get to know new languages in a deeper, more authentic way.

After a chat with the lead architect, you agreed on a series of unit tests that will guide functions you should write. Use a lodash method in each function – in each case, doing so will save you time and hassle. Each function will either manage data with Node (used to respond to API requests) or will make a request from the client using AJAX.

## Milestones

1. Clone [the repository](https://github.com/Thinkful-Ed/node-lodash) containing a starter point and some unit tests.

2. Install the project by running `npm install`.

3. Run the test suite using `npm test` to see the next test to complete.

4. Go through the `/src/` files starting with `01-*.js` and implement the functions one at a time by passing the tests. Take a look at the comments in each file describing the signature in more detail.

    1. `findCourseByName` - This function will be used for selecting a course from the list. Take a look at [`_.find`](https://lodash.com/docs#find).

    2. `findCoursesBySkills` - This function will need to select a list of courses that all offer the provided skill names. Take a look at [`_.chain`](https://lodash.com/docs#chain), [`_.filter`](https://lodash.com/docs#filter) and [`_.pluck`](https://lodash.com/docs#pluck) and [`_.intersection`](https://lodash.com/docs#intersection).

    3. `getGroupedCourses` - This function will return a nested array of courses grouped by language and sorted by the suitability of the language. Take a look at [`_.sortBy`](https://lodash.com/docs#sortBy) and [`_.where`](https://lodash.com/docs#where)

    4. `multiSort` - This function will return a list of courses sorted by multiple fields. Take a look at [`_.sortByAll`](https://lodash.com/docs#sortByAll) and [`_.includes`](https://lodash.com/docs#includes).

    5. `requestAdapter` - This file will expose 5 functions and you'll need to write 3 of them. Two of these functions will make use of the first. The first function is a requestAdapter that returns functions. Read up on [Partial Application and Composition](http://benalman.com/news/2012/09/partial-application-in-javascript/) and then take a look at [`_.partial`](https://lodash.com/docs#partial) and [`_.bind`](https://lodash.com/docs#bind).
 
5. Keep running the tests `npm test` to see if if your functions meet the requirements. If you get stuck, remember to log things out, also feel free to open the developer tools inside the `lodash` documentation webpage to play around with various `lodash` functions.

6. Try to make the code as eloquent and functional as possible to keep your hipster stakeholders happy.

7. Don't sneak peak at the `/solutions/` folder, and if you do - try to implement the solutions in a different way! Happy hacking!

## Resources

[Lodash Intro Video](https://egghead.io/lessons/core-javascript-introduction-to-lodash) - A short video introducing lodash/underscore and giving an example of chaining.

[Lodash Documentation](https://lodash.com/docs) - The fluffing lodash manual.

[Lodash Cookbook](https://leanpub.com/lodashcookbook/read) - Free on-line book containing many techniques and tips for when working with the lodash library.

[Partial Application and Composition](http://benalman.com/news/2012/09/partial-application-in-javascript/) - Detailed article on partial application and composition methods in JavaScript.
