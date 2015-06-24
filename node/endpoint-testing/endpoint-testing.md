
title:                  Record Profits: Endpoint Testing
description:            Help Amazon refactor their codebase by writing and testing the API endpoint for adding vinyl records to their list of products.
duration:               2 hours
skill_level:            Intermediate
core_concepts:          Node API Endpoints, Endpoint Testing
prerequisite_concepts:  [To come]

tags:                   Node
date_implemented:       [To come]
slug:                   [To come]

## Project Brief

Amazon have finally decided to enter the 21st Century and redesign their site as a single page application.  You have been tasked with writing and testing the API endpoint for adding vinyl records to their list of products.

### Creating the Endpoint

The endpoint should receive JSON data in the following format:

```json
{
    "artist": "Pavement",
    "album": "Slay Tracks (1933–1969)",
    "tracks": [
        {
            "title": "You're Killing Me",
            "length": 200
        },
        {
            "title": "Box Elder",
            "length": 146
        },
        {
            "title": "Maybe Maybe",
            "length": 134
        },
        {
            "title": "She Believes",
            "length": 182
        },
        {
            "title": "Prices Yeah!",
            "length": 180
        }
    ],
    "price": 146.94
}
```

In a frankly surprising move Amazon have decided that a flat-file database is the best way to store hundreds of millions of products, so your endpoint simply needs to write the JSON data out to a file.


### Testing the Endpoint

Importing the data from Amazon's old system is expected to be painful.  It is stored in various formats in a mixture of databases, and the import script is approaching 100,000 lines of code.  Therefore your endpoint needs to thoroughly check that the data is formatted correctly before entering it into the system.  Specifically:

* If the information which you are sent isn't JSON, then the endpoint should return a `415 Unsupported Media Type` error
* If the information which you are sent isn't valid JSON, then the endpoint should return a `400 Bad Request` error
* If a piece of information is missing (for example, a track does not have a title), then the endpoint should return a `422 Unprocessable Entity` error, with a description of which information is missing
* If a piece of information has the wrong type (for example if the artist name is an integer), then the endpoint should return a `422 Unprocessable Entity` error, with a description of which information is incorrect

## Milestones

1. Write a POST endpoint which parses the JSON from the post body, and writes it to a new file.  If you need some pointers then take a look at [this assignment on creating POST endpoints with Express](https://courses.thinkful.com/node-001v4/assignment/2.2.3).
2. Write a test for the endpoint which sends some data to the endpoint and checks to see whether the file has been written and contains the correct contents.  Take a look at [this lesson](https://courses.thinkful.com/node-001v4/lesson/2.3) for a guide to testing API endpoints using Mocha and Chai
3. Write additional tests which send different types of invalid data to the endpoint and check to see whether the appropriate errors are returned.  The [Chai HTTP documentation](http://chaijs.com/plugins/chai-http) covers the different types of assertions which you can make in your tests.
4. Update your endpoint to make your tests pass by validating the data using JavaScript.  For example, to check whether a piece of data exists you can look at the contents of the `request.body` object.

## Resources

* Completely new to testing?  Take a look at [this introduction to Behaviour-Driven Development](Introduction to Behavior-Driven Development with JS - Chapter 1), a popular methodology for automatically testing code.
* For an introduction to creating APIs in Node, work through [this lesson](https://courses.thinkful.com/node-001v4/lesson/2.2)
* Take a look at [how Twitter handle errors in their API](https://dev.twitter.com/overview/api/response-codes) for an example of a scheme for returning information about errors.

## Example Solution

[To come]