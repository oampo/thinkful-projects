title:                  Form-ing a Band: Form Handling and Servers  
description:            Write an app that outputs band names based on a user's selected genre. To do so, you'll learn to set up a basic Express server to work with user input.  
duration:               3 hours  
skill_level:            Intermediate  
core_concepts:          Node, servers, Express, form handling  
prerequisite_concepts:  Proficient with JavaScript, Creating Node servers  

tags:                   Node
date_implemented:       June 23, 2015  
slug:                   form-handling-and-servers  


##Project Brief

You've grown your [hair long](http://www.bbc.co.uk/staticarchive/ba447cda441cdf12b3c505c727e259343a1b2d1f.jpg).  You've got some [platform shoes](http://vignette2.wikia.nocookie.net/tron/images/8/82/Ziggy-stardust-david-bowie.jpg/revision/latest?cb=20101122042616).  You've got a [Marshall stack](http://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/MarshallStack_Slayer.jpg/1920px-MarshallStack_Slayer.jpg), a [sweet axe](http://proguitarshop.com/media/cms/blog/abstract-symbol-01.jpg), and [bags of attitude](http://cdn.smosh.com/sites/default/files/legacy.images/smosh-pit/092010/worstband-40.jpg).  That's right, you're [forming a band](https://www.youtube.com/watch?v=Nek-YO7v3Yw)!

But a great band is nothing without a great band name.  Would Megadeth have sold so many albums if they were called Medium-sized-deth?  I think not.  And who wants to spend the time thinking of a great name, when you can get a computer to do the hard work for you?

For this project you'll build a Node app to generate band name ideas and member pseudonyms for [power trio](http://en.wikipedia.org/wiki/Power_trio) bands playing different generes of music (e.g. Country, Heavy Metal, Jazz).

## Milestones

### Milestone 1: Creating the band name

For a gig in the back room of the local bar you should write an app which:

* Displays a form with buttons for different genres of music.
* Makes a request to the server when one of the buttons is clicked, passing in the genre.
* Generates a genre-appropriate band name
    - This can be done by adding together random start and end portions.  For example, for country the start part could be "The Ol' Time", "The Foggy Mountain", or "The Whiskey Drinkin'", and the end part could be "Hillbillies", "Boys", or "Bluegrass Band".  This would give band names such as "The Whisky Drinkin' Hillbillies", or "The Foggy Mountain Bluegrass Band".
* Shows a results page with the band name you've generated.

### Milestone 2: Give yourselves pseudonyms

For an 11AM slot at the Isle of Lucy Jazz-Blues Festival your app should generate and display suitable pseudonyms for each of your three members. You can use a similar technique to the genre generation using first and last names.  So for example a first name could be "Drinkin' Willie", and the last name could be "McGraw III", to give the name "Drinkin' Willie McGraw III".

### Milestone 3: More flexible band lineups

To sell out three nights at Madison Square Garden your app should:

* Allow the user to select how many members will be in the band and which instruments they'll play.
* Use the pseudonym generator to create a pseudonym for each member.
* Display the band name, along with the pseudonyms and instruments.

##Additional Resources

To complete this project, you'll want to be familiar with the following concepts:

- [Simple Express servers](https://courses.thinkful.com/node-001v4/assignment/2.1.1), which respond to HTTP requests.
- [Form Handling](https://courses.thinkful.com/oreilly-node-express/chapter/1.12).  You can use the body-parser to receive form data.
- [String Concatenation](https://courses.thinkful.com/node-001v4/assignment/1.1.2) for "gluing together" two strings.
- [GET Requests](https://courses.thinkful.com/node-001v4/assignment/2.2.2): for requesting data from a web server.

