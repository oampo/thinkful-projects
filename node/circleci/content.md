[Powers of ten are tricky right?](http://verizonmath.blogspot.co.uk/2006/12/verizon-doesnt-know-dollars-from-cents.html)  Well your boss at Apple wasn't happy last year when the website was listing the price of an iPad as $25,000.  And she is even less happy now she's found out that for the last 24 hours the website has been selling iPads for $2.50.

During a rather tense meeting you are told in no uncertain terms that if this happens again then you will be taking the first train out of Cupertino.  So to make sure that you aren't expelled from the campus, you decide that it's time to put some safeguards in place with a continuous deployment system.

## Milestones

### Milestone 1: Set up a test

In this milestone you are going to set up a test which makes sure that the prices returned from the endpoint fall within the correct power of ten.

To complete the milestone you should:

* Create a new project, and initialize it using `npm init`.
* Download the [code for the prices endpoint](https://gist.github.com/oampo/b343f27e5e9aa729f9ea).
* Install the dependencies: `npm install --save express` and `npm install --save-dev mocha chai chai-http`.
* Use Mocha and Chai to add a test which makes sure that the prices are within the correct power of ten.
    - The MacBook should be to the third power of ten.
    - The iPad should be to the first power of ten.
    - The iPad should be to the second power of ten.

Run your tests to make sure that the endpoint is working, and try changing the prices to make sure that your test fails.

#### Sample Code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/86634368a87e3ae47eb9).

### Milestone 2: Continuous testing

In this milestone you are going to set up CircleCI to run your tests every time you push your code.

First, update your `package.json` to tell the `test` script how to run your tests.  Push your code up to GitHub, and then activate the repository in the CircleCI dashboard.  You should see your tests running.  If the tests pass then you can move on to Milestone 3.  If they fail, then fix up the code and push it up to GitHub again to make sure that your build on CircleCI is green.

### Milestone 3: Deploy to Heroku

To complete this milestone you should set up the endpoint so that it is deployed on a Heroku dyno.

### Milestone 4: Continuous deployment

In this milestone you are going to set up CircleCI to continuously deploy your app when you push changes to GitHub.  Set up CircleCI so that it can deploy app to Heroku, then add a `circle.yml` file describing the deployment of your app.  Push the `circle.yml` file up to GitHub.  You should see an extra stage added to your build process which automatically pushes the code up to Heroku if the build succeeds.

## Additional resources

[This blog post](http://blogs.atlassian.com/2014/04/practical-continuous-deployment/) looks at best practices when running continuous deployment on a production app.
