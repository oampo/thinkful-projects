Following [The Button's](https://en.wikipedia.org/wiki/The_Button_%28Reddit%29) [untimely demise](http://www.redditblog.com/2015/06/the-button-has-ended.html), your hand, tired of hovering over your mouse waiting to click, has been [acting kind-of strangely](https://www.youtube.com/watch?v=sDentLWRoSQ).  Your physician recommends the you immediately recreate the button as a CLI app, so you can finally rest your weary hand.

# Milestones

## Milestone 1: Sign up for Firebase

In this milestone you will sign up for [Firebase](https://www.firebase.com/) and explore it's user interface.  Firebase is the real-time database which you will be using to record the clicks.

To complete the milestone you should:

* Sign up with [Firebase](https://www.firebase.com)
* Create a new app called "Button"
* Click the "Manage App" to administer your app

In the app dashboard you should see a display where you can add and explore the data held in your application.  You can use this to view the state of your application at any time.

Also take a look at the "Security and Rules" tab.  This is where you add the rules which keep your app secure, and validate your data.

## Milestone 2: Pushing the button

To complete this milestone you should:

* Create a new project called *firebase-button*, and run `npm init`.
* Install the Firebase module (`npm install firebase`).
* Create a new script called *push.js*.

The *push.js* script should connect to the database, and set the value of an reference called `button`.  This should be set to an object which contains [the timestamp on the server](https://www.firebase.com/docs/web/api/servervalue/timestamp.html).  The script should then exit.

After running the script your database should look something like this:

```json
{
    "button": {
        "timestamp": 1234567890
    }
}
```

When you run the script again, the timestamp should update to the new time.

### Sample code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/5ff4cf89db29777576bf).

## Milestone 3: Watching the button

Create a new script called *watch.js*.  To complete this milestone, the script should connect to the database, and watch for changes to the `button` reference.  When there is a change, the script should print out a notification that the button was pressed, and how long there was to spare before the 60 seconds ran out.

### Sample code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/61fe96d8d26f23bb586e).

## Milestone 4: Secure the button

Currently you'll notice that you can still push the button even after the 60 seconds has passed.  Your watch script may give you some interesting output in this case.  So, to complete this final milestone you should add some rules to the database which enforce the following conditions:

* The new button data should have a `timestamp` attribute
* The value of the `timestamp` attribute should be a number
* If there is existing data in the button element, then the difference between the two timestamps should be no more than 60 seconds, and no less than 0 seconds.
* The timestamp should be equal to the current server timestamp.

### Sample rules

When you have completed the milestone, compare your rules to [this set of sample rules](https://gist.github.com/oampo/1138e46d8d5543c89858).


# Resources

* The [Firebase guide](https://www.firebase.com/docs/web/guide/) provides a great introduction to all-things Firebase.
* Want to understand the Firebase security model better?  [This example](https://gist.github.com/katowulf/4741111) of some rules for a simple chat application provides a series of insights into how data can be secured and validate.
