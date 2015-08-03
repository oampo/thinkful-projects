## Read & Watch

Before diving into the project below, take a read of the following resources:

* [This guide](http://eddywashere.com/blog/swig-for-designers/) takes you through the essential syntax of [Swig](http://paularmstrong.github.io/swig/), the templating engine which you will be using for this project.
* The Swig documentation has a [guide to using Swig with Express](http://paularmstrong.github.io/swig/docs/#express) which will come in handy for the first milestone.

## Build

[Philip Roth](https://en.wikipedia.org/wiki/Philip_Roth), one of America's most accomplished literary award winners, has been struggling to get his new novel off the ground.  As a last resort, he has decided that all of his future novels will be written using an ingenious system which he calls [Mad Libs](https://en.wikipedia.org/wiki/Mad_Libs).

In Mad Libs you simply replace the blanks in a story with words which fit into a certain category.  For example:

```
"_____________! he said ________ as he jumped into his convertible
   exclamation            adverb
 ______ and drove off with his __________ wife."
   noun                         adjective
```

With the words completed, the sentence might read:

```
"Ouch! he said stupidly as he jumped into his convertible
cat and drove off with his brave wife."
```

You have been tasked with helping Mr Roth out by creating an app for him to tinker with his Mad Libbed creations.

## Milestones

### Milestone 1: Set up Swig

In this milestone you are going to create an Express application using Swig as the templating engine.

To complete the milestone you should:

* Create a new project, and initialize it using `npm init`.
* Install Express and Swig using `npm install --save express swig`.
* Create a file called `index.js` which initializes a new Express app.
* Configure the app to use Swig as its templating engine.
* Create a `/` endpoint which uses `res.render` to serve a simple "Hello World" template from your template directory.

#### Sample Code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/5529ddcd773eddb82a9f).

### Milestone 2: Add the mad-libs form

To complete this milestone you should add a form to your template which makes a post request to the `/` endpoint.  The form should have spaces to fill in each of the gaps in the Mad Lib.  You can customize these yourself, or use the following list:

> A Female Name, A Dirty Task, An Obnoxious Celebrity, A Job Title, A Celebrity, A Huge Number, A Tedious Task, A Useless Skill, An Adjective

You will need to install and use the [body-parser module](https://github.com/expressjs/body-parser) to parse the form data.  If you haven't looked at working with forms before, then don't worry - you simple need to `app.use(bodyParser.urlencoded());`, and your requests will have a `req.body` containing your form data.

#### Sample code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/869b88f25f45ed26899c).

### Milestone 3: Render the output

In this milestone you will create the template which contains the story, and fill it with the phrases from your form.

To complete the milestone you should:

* Create the post endpoint for `/`, which renders a story template.
* Create the story template, with placeholders for the phrases.
* Pass the contents of `req.body` into the template to fill in the phrases.

You can either make up a story to match your customized form data, or use the story below:

```
____________________ was a ____________________ who loved technology. Although
         Female Name                  Job Title
she loved parts of her job, she absolutely hated ____________________
                                                         Tedious Task
and ____________________. So, ____________________ met with her life mentor
              Dirty Task               Female Name

____________________ who told her to learn how to ____________________ with
           Celebrity                                     Useless Skill

Thinkful. Thinkful didn't offer a course on _____________________ so she
                                                    Useless Skill
studied programming instead.

What a great decision! With her new skills, ____________________ built a(n)
                                                     Female Name
_____________________ robot named ____________________ that not only loved
            Adjective              Obnoxious Celebrity
_____________________ but did it _____________________ times faster.
           Dirty Task                      Huge Number
```

Test out your code by filling in the form, and taking a look at your _meisterwerk_.

#### Sample Code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/8bc4b996e4b89123feb0).

## Additional Reading

There are a whole host of other templating engines out there which you may want to explore.  The choice of engine comes down to personal preference to a large part.  Some of the more prominent engines are:

* [Jade](http://jade-lang.com/)
* [Handlebars](http://handlebarsjs.com/)
* [EJS](https://github.com/tj/ejs)
