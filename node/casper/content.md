## Read & Watch

Before you get started on the project, take some time to read [this article](http://www.helpscout.net/blog/functional-testing-casperjs/).  It provides an introduction to CasperJS, the browser automation framework which you will be using in this project, and a worked example of using it to test Reddit.


* [The CasperJS testing documentation](http://casperjs.readthedocs.org/en/latest/testing.html)

## Build

The Stack Overflow Careers site is having an intermittent reliability issue caused, ironically, by a stack overflow. After two weeks of trying to diagnose the problem, Joel Spolsky himself has stepped up to the plate and found a solution.  So for the last week Joel has sat within arms reach of a laptop, and performed a search on the site every 60 seconds.  If the search fails then he hits the big red button and restarts the server.  That's 10080 searches and counting.

In this project you will try to relieve Mr Atwood from his duties by writing an automated test which uses [CasperJS](http://casperjs.org/) to check to see whether the search functionality is working.

## Milestones

### Milestone 1: Hitting the front page

In this milestone you are going to set up a Casper test case which visits [the Stack Overflow Careers front page](http://careers.stackoverflow.com), and checks that you are seeing the correct page.  To complete the milestone you should:

* Create a new project
* Install CasperJS (`npm install --save -g casperjs`)
* Set up a new Casper suite which:
    - Visits http://careers.stackoverflow.com
    - Checks that the title of the page is the string "Stack Overflow Careers"

If you need a reminder on how to set up Casper tests, take a look at [the testing documentation](http://casperjs.readthedocs.org/en/latest/testing.html).

Run your test to make sure that you are retrieving the front page successfully.

#### Sample code

When you have completed this milestone, compare your code with [this sample code](https://gist.github.com/oampo/6687dba4d40ad740ede4).

### Milestone 2: Performing the search

To complete this milestone you should extend your test suite so that it performs a search for the keyword "node.js".  Your test will need to find and fill in the search form, submit it, and wait for the results to be returned.

When the results are returned, you should check that the title of the page has been updated to reflect your search.

#### Sample code

When you have completed this milestone, compare your code with [this sample code](https://gist.github.com/oampo/cc8f50ae724ad00b858e).

### Milestone 3: Checking the results

When the search is complete the site displays the number of search results in a `<span>`.  To make sure that the search functionality is working you should extend your tests to make sure that the number of results is greater than zero.

#### Sample code

When you have completed this milestone, compare your code with [this sample code](https://gist.github.com/oampo/e57664f623582b5f75fb).


### Milestone 4: Test another feature

In this milestone you should add a test for another feature of the StackOverflow Careers site.  This could be any feature you like, but if you are stuck for ideas here are a few suggestions:

* Make sure that searching for a keyword only returns results which contain that keyword.
* Make sure that the "Allows remote" button only returns remote positions.
* Check that clicking on a job advert takes you to a complete description of the job.

## Additional Resources

* CasperJS is built on top of [PhantomJS](http://phantomjs.org/).  If you are interested in the technology behind the scenes then check out [this quick start guide](http://phantomjs.org/quick-start.html).

