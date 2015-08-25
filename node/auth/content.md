## Build

The Chaos Computer Club is a [hot new social network](https://en.wikipedia.org/wiki/Chaos_Computer_Club) for coders.   Following a $1 million seed round from Peter Thiel , a $100 million series A investment led by Andreessen Horowitz, and a $2 Billion IPO, they have decided that it's time to write some code.  And what better place to start than the user creation and authentication system?

## Milestones

### Milestone 1: Create the user model

Create a model to represent a user.  The model should store a username and a password which is hashed using [the `bcrypt` library](https://www.npmjs.com/package/bcrypt).  You should be able to set the password (which will hash and store the new password), and check a password against the stored hash.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/2870fcf65f4731e78598).

### Milestone 2: Add a registration endpoint

Set up an Express application, and add a `/register` endpoint.  This should take a username and password sent by the user as JSON data, and use them to create and store a new `User` object.  Test this out by using cURL to create a new user.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/1f17192f4e4dc56033c6).

### Milestone 3: Add the authentication strategy

Use [passport.js](http://passportjs.org/) to add a basic access authentication strategy to your app.  This should check whether the supplied password matches the stored password for a given user.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/2fae78e5af5392b6e2bb).

### Milestone 4: Protect an endpoint

Create an endpoint which returns a welcome message to an authenticated user.  The endpoint should be protected using the basic auth strategy.  Test this out by using cURL to visit the endpoint without providing login credentials.  This should tell you that you are unauthorized.  Then try again, supplying the correct credentials.  You should see your message.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/13febebd5767ef251960).
