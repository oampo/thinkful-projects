title:                  RESTful Books
description:            Implement a RESTful API for UBaaS: Used Books as a Service
duration:               4-8 hours
skill_level:            Advanced
core_concepts:          REST, Express, Node.js
prerequisite_concepts:  URIs, JSON, node.js, Express
tags:                   <!-- Leave this empty -->
date_implemented:       <!-- Leave this empty -->
slug:                   <!-- Leave this empty -->

## Project Brief

You are the proprietor of _Very Good Used Book Store, LLC_, the best used book store in the Upper Midwest, and you want to expand your business.  You've been reading about startups, and you think the market is ready for a new concept: Used Books as a Service (UBaaS). You've determined that the Minimum Viable Product must provide a way for applications to:

* search for books by _title_, _author_, _publisher_, _price_, or _ISBN_.

* list books in stock by _title_, _author_, _publisher_. (Remember you have thousands of books in stock, so make sure you can limit the number of books in each request)

Once you've demonstrated the MVP, extend it by adding operations to let you manage the inventory.

## Resources

To complete this project, you'll want to be familiar with the following concepts and resources:

* Building a new node.js project using Express

    * This shows how to set up a new project, if you need a reminder. [Hello KnoBe](https://projects.thinkful.com/12/)

* ReST: Representational State Transfer

    * A short light-hearted explanation. [How I explained REST to my wife](http://www.looah.com/source/view/2284)

    * A better shoirt explanation. [A Brief Introduction to REST](http://www.infoq.com/articles/rest-introduction)

    * A good tutorial. [Learn REST: A Tutorial](http://rest.elkstein.org/)


    * The answers to [this Stack Overflow question](http://stackoverflow.com/questions/671118/what-exactly-is-restful-programming) explain ReST well.

    * Chapter 5 of Roy Fielding's dissertation [defining ReST](http://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm) is the ultimate resource.

    * Understanding how the _representation_ has all the _state_ is a ket to understanding ReST. [Approaching Pure REST](http://kinderman.net/2010/06/23/approaching-pure-rest-learning-to-love-hateoas)

    * You can steal a lot of code from this if you're thoughtful. [Build a RESTful API using node and Express 4](https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4)

* Testing your API

    * _cURL_ is the standard command-line tool for manipulating HTTP. Everyone should know about it, but it's arcane. [How to test a REST API with cURL](http://www.codingpedia.org/ama/how-to-test-a-rest-api-from-command-line-with-curl/)

    * [The Httpie Tool](https://pypi.python.org/pypi/httpie) is a very useful command line tool for testing APIs and for exploring HTTP in general.

    * _Postman_ is a browser-based tool for API testing.  Set up your API calls and see what happens. [Using Postman](https://www.getpostman.com/docs/blog_mentions)

    * This is a tutorial for both _Postman_ and _HTTPie_. [POSTMAN and HTTPie to test APIs](http://blog.mashape.com/postman-httpie-test-apis/)

## Milestones

### Milestone 1: Make a Catalog

* Define a JSON format for your book catalog.

* Create some test data.  (This project is concentrating on APIs, so it's okay to just store your test data in a literal object, but if you are comfortable with MongoDB, you might instead set up a MongoDB collection.)

* Define your API for both listing and searching, and document it by identifying the CRUD operations and the HTTP verbs that match those operations for your APIs. (Note that so far we *haven't* specified anything except READ operations.)

### Milestone 2: Implement your MVP

* Create a new node.js project including Express and (optionally) Mongoose. 

* Implement each of the URI routes defined for your MVP.

* Test your API using Postman, _curl_ or _httpie_.

### Milestone 3: Update the Catalog

Now that you have your MVP, you would like to be able to add the following operations: add a book, update the number of copies in stock, delete a book, and change the price.

* Update your API documentation for each of the new operations.

* Modify your implementation to support each new operation.

### Milestone 4: Sell a Book

* Add operations to sell a book

* Sell a book.


