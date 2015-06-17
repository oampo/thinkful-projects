Level: Intermediate
Time Estimate: 2 hours
Topics: Testing API endpoints, Mocha, Chai, Handling JSON, API error codes

# Project Brief

Amazon have finally decided to enter the 21st Century and redesign their site as a single page application.  You have been tasked with writing and testing the API endpoint for adding vinyl records to their list of products.

The endpoint should receive JSON data in the following format:

```json
{
    "artist": "Pavement",
    "album": "Slay Tracks (1933–1969)",
    "tracks": [
        {
            "title": "You"re Killing Me",
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
    price: 146.94
}
```

In a frankly surprising move Amazon have decided that a flat-file database is the best way to store hundreds of millions of products, so your endpoint simply needs to write the JSON data out to a file.

Importing the data from the old system is expected to be painful.  It is stored in various formats in a mixture of database, and the import script is approaching 100,000 lines of code.  Therefore your endpoint needs to thoroughly check that the data is formatted correctly before entering it into the system.  Specifically:

* If the information which you are sent isn't JSON, then the endpoint should return a `415 Unsupported Media Type` error
* If the information which you are sent isn't valid JSON, then the endpoint should return a `400 Bad Request` error
* If a piece of information is missing (for example, a track does not have a title), then the endpoint should return a `422 Unprocessable Entity` error, with a description of which information is missing
* If a piece of information has the wrong type (for example if the artist name is an integer), then the endpoint should return a `422 Unprocessable Entity` error, with a description of which information is incorrect

# Milestones

1. Write a simply PUT endpoint which doesn't worry about error checking, and simply writes the JSON to a file.
2. Write a test for the endpoint which sends some data to the endpoint, and checks to see whether the file has been written and contains the correct contents.  Take a look at [this lesson](https://courses.thinkful.com/node-001v4/lesson/2.3) for a guide to testing API endpoints using Mocha and Chai.
3. Write some further tests which send different types of invalid data to the endpoint and check to see whether the appropriate errors are returned.
4. Update your endpoint to make your tests pass.

# Resources

* For an introduction to creating APIs in Node, work through [this lesson](https://courses.thinkful.com/node-001v4/lesson/2.2)
* Take a look at [how Twitter handle errors in their API](https://dev.twitter.com/overview/api/response-codes) for an example of a scheme for returning information about errors.

