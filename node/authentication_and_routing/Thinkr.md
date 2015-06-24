title: The Social Notwork: Authentication and Routing
description: Create the next big thing. Build a simple social network to learn the basics of Node with Express. Set up authentication, work with a Mongo database, and learn how Node works with templating engines.
duration: 12 hours
date_implemented: June 23, 2015
skill_level: Advanced
slug: thinkr
tags: Node
 

Concepts: Node, servers, Express, MongoDB, Authentication, Templating
Pre-reqs: Proficient with JavaScript, Creating Node servers

##Project Brief

This project has you build a simple web application to learn the basics of Node with Express. You'll set up authentication, work with a Mongo database, and learn how Node works with templating engines. You should already be comfortable programming in JavaScript and understand MVC frameworks, but no prior Node experience is required.

Thinkr is the hot new social network which lets you tell the world what you are thinking in Thoughts: messages made up of 4 characters or fewer.  A $1 million seed round from Peter Thiel was followed by sustained exponential growth over a 24 hour period.  This led to a $100 million series A investment led by Andreessen Horowitz which valued the company at a little over $1 billion.  Two weeks later and Thinkr is preparing for the largest IPO in stock market history.

However there is one small hitch.  A disgruntled TechCrunch journalist has written a stinging exposé revealing that the Thinkr team don't have a single line of code written.  At short notice you have been called in to remedy the situation by creating the Thinkr backend from scratch using Node.js, Express and MongoDB.

##Milestones

### Milestone 1: Authentication, writing and reading thoughts

To secure an IPO of $30 billion your backend should:

* Allow users to sign up and log in
    - The [Passport.js](http://passportjs.org) library contains code to simplify the authentication process
* Allow users to post messages consisting of 4 characters or fewer.  Posts longer than 4 characters are considered a thought crime, and should respond with an appropriate error message.
* Show the last 20 Thoughts of a specific user

### Milestone 2: Following users and a timeline

For a $50 billion IPO your backend should:

* Allow users to follow and unfollow other users
* Show users the last 100 thoughts from the users who they follow

### Milestone 3: Hashtags and trending thoughts

For a $100 billion IPO your backend should:

* Support lists of trending thoughts that users can read.  Thoughts should trend when they are expressed by more than three users within the last 10 minutes.
* Let users search all thoughts by hashtag.  Because who needs four characters when you can express your thoughts in #thr...ee?


##Additional Resources

To complete this project, you'll want to be familiar with the following concepts:

- [Authentication](https://courses.thinkful.com/oreilly-node-express/subsection/1.22.2): Authentication refers to knowing who is who and verifying users' identities. You'll want to be able to securely store usernames, passwords, and email addresses for this project. As mentioned, using Passport.js will save you time and provide best practices for user management.
- [GET Requests](https://courses.thinkful.com/node-001v4/assignment/2.2.2): A GET request is a web request soliciting data.
- [POST Requests](https://courses.thinkful.com/node-001v4/assignment/2.2.3): A POST request is the kind we use when we actually want to submit information to the web for it to be stored or acted upon, such as when we want to add a new thought.
- [Saving Time with Express](https://courses.thinkful.com/oreilly-node-express/chapter/1.7): This chapter introduces setting up a server with Express. Express will help you define the internal structure of your application, define which pages you need, and what each page does.
- [Form Handling](https://courses.thinkful.com/oreilly-node-express/chapter/1.12): This chapter will teach you how to collect, receive and validate information from users.
- [Introduction to MongoDB](https://courses.thinkful.com/node-001v4/assignment/3.1.1): Using MongoDB as the database will help you keep track of all users, thoughts and hashtags in Thinkr.
- [Introduction to Mongoose](https://courses.thinkful.com/node-001v4/assignment/3.1.2): Mongoose is the most popular Object Document Mapper for MongoDB. It'll help you model and validate your data more efficiently. 
- [Deploying to Heroku](https://courses.thinkful.com/node-001v4/project/2.2.5): For a simple app like this one, deploying to Heroku is the fastest way to get it live on the web. Heroku is a layer of abstraction on top of Amazon Web Services that lets you avoid setting up your own server from scratch.
- Bonus: [Templating with Handlebars](https://courses.thinkful.com/oreilly-node-express/chapter/1.11): Handlebars (or Jade, which is introduced in the same chapter) is the most popular templating engine used with Node. You can use it to easily include dynamic information (new thoughts or hashtags) in your HTML templates.
