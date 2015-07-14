A paranoid billionaire going by the pseudonym Lobby Lud has been busy exercising his [right to be forgotten](https://en.wikipedia.org/wiki/Right_to_be_forgotten).  To make extra sure that no trace is left on the internet, he has offered a bounty of $1 million to anyone who can work out his true identity.

But you have worked out a plan.  You are going to send Mr Lud an email explaining that you are a [wealthy aristocrat who has been imprisoned in Spain](https://en.wikipedia.org/wiki/Spanish_Prisoner).  To secure your release, all Mr Lud needs to do is to sign into a web app using his Google account, and press the "Release Prisoner" button.  On your release you will promise to shower Mr Lud with even greater riches.  But actually you are going to find out his identity through his Google account and [claim the $1 million all for yourself](http://i.giphy.com/ZvsIuK3ovaHoA.gif).

# Milestones

## Milestone 1: Register a new app with Google

To complete this milestone you should:

* Create a new empty project from the [Google Developer's console](https://console.developers.google.com/project).
* When the project is created select the "APIs and Auth" tab, then go to the APIs tab. Click on the Google+ API, and enable the API.
* Next, click on the Credentials tab, and click "Create a new client ID", selecting the Web Application type.  You will be asked to name the project.  Then in the "Authorized JavaScript origins" box, enter `http://127.0.0.1:8080`, and in the "Authorized redirect URIs" box, enter `http://127.0.0.1:8080/authenticate/callback`.  When this is done you should see a Client ID and Client Secret have been created.

## Milestone 2: Create the app

Create a simple Express project with four GET endpoints:

* `/` - This should display a log in link, pointing to `/authenticate`
* `/authenticate` - This should be blank for now
* `/authenticate/callback` - This should also be blank for now
* `/display`
    - If an attribute `req.user` exists in the request object, then this should display the string `"You are {{ username }}, and I claim my $1 million"`, where `{{ username }}` should be replaced with `req.user.displayName`.
    - If an attribute `req.user` does not exist, then the user should be redirected to the `/authenticate` route.

## Milestone 3: Add authentication

Use [passport](http://passportjs.org/), and the [passport-google-oauth](https://github.com/jaredhanson/passport-google-oauth) library to add Google OAuth2 authentication to the application.

* You will need to use the client ID and secret from the developer console to set up your authentication strategy.
* The strategy should use the profile object returned by Google to represent the user.
* The `/authenticate` endpoint should try to authenticate with Google.
    - You will need to use the following scope to obtain the correct profile information: https://www.googleapis.com/auth/userinfo.profile
* The `/authenticate/callback` endpoint should handle the callback from Google, redirecting to `/display` on success, and `/authenticate` on failure.
* You will need to configure express and passport to save the profile object to the session.
* You will need to add functions to serialize and deserialize the profile object from the session.  These should simply call the `done` callback with the user object.

# Resources

* [The passport.js documentation](http://passportjs.org/docs) provides a wealth of information about the different stages of setting up authorization.
* The passport-google-oauth module provides [an example app](https://github.com/jaredhanson/passport-google-oauth/tree/master/examples/oauth2) to show how authentication using Google can be set up.
* The [beginner's guide to OAuth](http://hueniverse.com/oauth/) provides some information about how OAuth works, and why it is secure.

# Sample code

When you are done, take a look at the [sample code for the project](https://gist.github.com/oampo/a6f2694f9223c3826b83).


