## Watch & Read

* [Unit Testing: Why Bother](http://soundsoftware.ac.uk/unit-testing-why-bother/) is a great article on what unit testing involves, and why it is useful.
* [This video](https://www.youtube.com/watch?v=zMJ4BAE1ACA) shows how Mocha, the unit testing framework which you will use in this project, can be used to add tests for a new feature in a blackjack application.
* [This article](http://nelsonic.gitbooks.io/node-js-by-example/content/core/assert/README.html) gives an introduction to the methods in the Node.js `assert` library, which you will be using to ensure that your code is behaving correctly.

## Build

A second dot-com crash has seen your company's valuation dropping from $1 billion to $100 overnight, leaving you and your co-workers seeking employment.  Rather than find another programming gig, you and your colleagues decide to turn your hand to bank robbery.

Before you start casing the join for your first big score, you need to work out how to split the loot.

Curly, formerly your project manager, suggests that you submit weekly timesheets, and the money will be divided according to how long you each worked.

Larry, the junior developer, writes a [short Node.js function](https://gist.github.com/oampo/eef075f95e77f14573d5) to work out the split.

Moe, a [TDD](https://en.wikipedia.org/wiki/Test-driven_development) enthusiast, complains that there are no tests written for the script, and says that he can't trust that he'll receive his fair share.

So it has been left to you to write tests which will convince Moe that the code is as bulletproof as the vests which you will soon be donning.

## Milestones

### Milestone 1: Setting up the test environment

In this milestone you are going to set up your test environment using Mocha, and add an empty test suite.

To complete the milestone you should:

* Create a new project, and initialize it with `npm init`.
* Copy [the untested code](https://gist.github.com/oampo/eef075f95e77f14573d5) into your project.
* Install Mocha using `npm install --save-dev -g mocha`.
* Create a file called `test.js`, and add a new empty test suite for the `splitLoot` function using Mocha's `describe` function.
* Try out the empty test suite by running it using `mocha test.js`.

The [Mocha getting started guide](http://mochajs.org/#getting-started) shows the basic syntax for setting up test cases.

#### Sample Code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/2366e2db1f76a14d587d).

### Milestone 2: Describe the program

To complete this milestone you should stub out a series of empty tests in your test suite, describing the behavior of the `splitLoot` function.  Try to cover both the obvious usages (for example, you steal $1,000,000, and everyone works equally hard), and the edge cases (for example, what should happen if you accidentally say that someone worked a negative number of hours).

#### Sample Code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/d9fcab8742e21c9f99dd).

### Milestone 3: Fill in the tests

To complete this milestone you should fill the detail of your test cases, using the `assert` module to make sure that your function is behaving correctly.  As you work through the tests you may need to modify the original function to improve its behavior in edge cases.

#### Sample Code

When you have completed this milestone, take a look at [this sample code](https://gist.github.com/oampo/88196f28e92656ecef17).

