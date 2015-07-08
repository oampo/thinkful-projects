title:                  Space Jam: Save NASA Using External API's  
description:            Use Node to interact with third-party API's to save the International Space Station.  
duration:               12 hours  
skill_level:            Intermediate  
core_concepts:          Node, servers, Express, Form handling, HTTP Clients, Making requests to APIs, Templating, Asynchronous programming  
prerequisite_concepts:  Proficiency with JavaScript, Creating Node servers, HTML  

tags:                   Node  
date_implemented:       June 23, 2015  
slug:                   external-apis-in-node  


## Project Brief

Following the latest round of budget cuts, NASA was forced to "dehire" a number of members of staff.  As the last engineer packed her box and headed for the exit, she helpfully pointed out to her project manager that she was the last person at NASA who knew the location of the International Space Station (ISS).  And that the GPS on board the ISS was on the fritz.

The Administrator of NASA took charge of the situation immediately, realizing the damage that losing $150 billion worth of space station could do to his reputation, not to mention his retirement fund.  Rather than crunching the numbers to work out where the ISS had got to, the Administrator ordered the construction of a giant cannon to fling a new GPS to the waiting ISS crew.

The cannon was built in record time, coming in only three years late and $5 billion over budget.  Now all that needs to be done is to work out when the ISS is going to be overhead, and fire the cannon.  And that is where you have been called in.

## Resources

To complete this project, you'll want to be familiar with the following concepts:

- [Making HTTP Requests](https://courses.thinkful.com/node-001v4/assignment/2.1.3): How to use Unirest to make HTTP requests to receive data from an API.
- [GET Requests](https://courses.thinkful.com/node-001v4/assignment/2.2.2): A GET request is a web request soliciting data.
- [Form Handling](https://courses.thinkful.com/oreilly-node-express/chapter/1.12): This chapter will teach you how to collect, receive and validate information from users.
- [Deploying to Heroku](https://courses.thinkful.com/node-001v4/project/2.2.5): For a simple app like this one, deploying to Heroku is the fastest way to get it live on the web. Heroku is a layer of abstraction on top of Amazon Web Services that lets you avoid setting up your own server from scratch.
- [Templating with Handlebars](https://courses.thinkful.com/oreilly-node-express/chapter/1.11): Handlebars (or Jade, which is introduced in the same chapter) is the most popular templating engine used with Node. You can use it to easily include dynamic information (new thoughts or hashtags) in your HTML templates.
- [Running async tasks in series](https://courses.thinkful.com/node-001v4/project/4.2.4): How to run one asynchronous task after another has finished
- [Running async tasks in parallel](https://courses.thinkful.com/node-001v4/assignment/4.3.1): How to run asynchronous tasks simultaneously, continuing when they have all finished.

## Milestones

### Milestone 1: Determine when the ISS passes overhead

To save the Administrator's bacon you need to write an app which:

* Has a simple HTML form with two inputs, one for latitude and one for longitude.
* When the form is submitted it should use Node.js to make a request to the [Open Notify ISS Pass Time API](http://open-notify.org/Open-Notify-API/ISS-Pass-Times/) with the supplied latitude and longitude.
* When the API responds your app should:
    - Convert the risetime to a human-readable date and time using the [JavaScript Date object](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Date)
    - Display the date and time of the next passes of the ISS in a results page

### Milestone 2: Converting a location to latitude/longitude

To secure the Administrator's job for the next 5 years your app should:

* Take the name of a location rather than a latitude/longitude pair.
* Use the [MapQuest Nominatim API](http://open.mapquestapi.com/nominatim/) to search for the location.
* Take the longitude and latitude of the best match from Nominatim, and use that as the input for the Open Notify API.

### Milestone 3: Checking the weather

To get the Administrator a healthy raise at his next pay review your app should:

* Use the [Yahoo Weather API](https://developer.yahoo.com/weather/) to retrieve the weather conditions for the location on the potential firing dates.
* Display the forecasts on the results page.


## Example Solution

Our solution is coming soon. Want us to take a look at yours? [Email us](dan@thinkful.com) a link to the GitHub project or share it on [Slack](https://thinkful-students.slack.com).
