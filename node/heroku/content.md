After months of market research you have finally found the product which the internet is crying out for.  A [lorum ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) generator.  Which says [Hodor](https://tctechcrunch2011.files.wordpress.com/2014/06/hodor-1024.png?w=738).

With the app completed, it's time to get it live on the World Wide Web.  And for a simple hosting solution it's hard to look beyond [Heroku](https://www.heroku.com/).

## Milestone 1: Install Heroku

To complete this milestone you should install the [Heroku toolbelt](https://toolbelt.heroku.com).  This gives you access to the `heroku` command line client, which you can use to create and deploy apps on Heroku.

## Milestone 2: Set up `package.json`

For Node.js apps, Heroku tries to install the dependencies by running `npm install`, and then tries to run the app using `npm start`.  For this to work, you need an up-to-date `package.json` file.

To complete this milestone you should:

* Create a new project and run `npm init`
* Download the source code for the Hodor generator from [this gist](https://gist.github.com/oampo/63f9f4d7f066d67a8d67).
* Install the app's dependencies, making sure to save them in your `package.json`.
* Add a `start` script to your `package.json` which describes how to run the app.

Try running the app locally to make sure it is working, then commit your changes to a git repository.

## Milestone 3: Push your app live

In this milestone you are going to push the app live to Heroku.  Create a new Heroku app using `heroku create`, then push the app up to the new `heroku` remote.

To check that this has worked, you can run `heroku open` to visit the site.


