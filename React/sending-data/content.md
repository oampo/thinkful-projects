## Build

Rantr is a new service which allows you to submit long irate rants.  The rants will be printed out, read by a sympathetic employee, and filed in the garbage.  Unfortunately the lead developer quit the project, promising to submitting a 10 page diatribe as soon as the app is complete.  So it is up to you to finish up the form handling, and make the app submit the rants to an API.

## Milestones

### Milestone 1: Render the tags

In the [current code base](http://codepen.io/jturner-thinkful/pen/PPYmyW) there is a completed component which allows you to select tags for how you are feeling.  This isn't being rendered as part of the form yet.  To complete this milestone you should add the `TagInput` component to the `MessageForm`, setting the `tags` list to an initial list of emotions to test it out.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/EVYmeM).

### Milestone 2: Make the tags update

The `TagInput` component has an `onTagAdd` property, which is called when the user creates a new tag.  Hook this up to a callback, and use it to update a list of tags held in the `MessageForm`'s state.  Then update the `TagInput` props so that it always reflects the contents of the tags state.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/jbNmvZ).

### Milestone 3: Submit the state to the API

When the form is submitted it should make an Ajax request to an API to submit the rant.  Currently the API is incomplete, so for testing you have been told to use [PutsReq](http://putsreq.com), a service which lets you record HTTP requests.

Use [axios](https://github.com/mzabriskie/axios), or an HTTP library of your choice, to make a POST request containing the contents of the `MessageForm` state to a new PutsReq.  Check that your code is working by submitting a rant, and making sure that it has been recorded in the PutsReq.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](http://codepen.io/jturner-thinkful/pen/qOWmye).

