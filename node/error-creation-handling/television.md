title:                  Working Remotely: Error Creation Handling
description:            Create error objects to handle errors for a 'Smart TV' JavaScript API. 
duration:               1 hour
skill_level:            Beginner
core_concepts:          Error handling, Callbacks, Inheritance
prerequisite_concepts:  [To come]


tags: Node
date_implemented:       [To come]
slug:                   [To come]


## Project Brief

The new Samsung Smart TV features 4-D images, 8-D sound, hyper-HD technology, and best of all, a JavaScript API.  Reliability on the early models isn't great, so you have been asked to implement the error handling code for [the JavaScript API](https://gist.github.com/oampo/5c76f5df3bcb7ee8cc8d).

To help you out the chief engineer has printed out a copy of the troubleshooting section of the user manual.  You should base the API's error handling on this manual:

> If your television will not switch on you may have one of the following problems:
>
> * *Unable to power television on (I)* - If you are unable to power on your television you have a faulty plug socket.  Insert a metal fork or thin conductive object into the socket.
>     - Error classification: TV Error
> * *Unable to power television on (II)* - If you are unable to power on your television then the power switch is broken.  Hotwire the switch, while pretending that your television is a 1964 Ford Cortina.
>     - Error classification: TV Error
> * *Unable to Change Channels (I)* - If you are unable to change channels then you have lost the remote control.  Vacate the sofa and search for it.
>     - Error classification: Environment error
> * *Unable to Change Channels (II)* - If you are unable to change channels then you have removed the batteries in order to power your [wall-mounted singing bass ornament](https://www.youtube.com/watch?v=XhB6ifx1B4A).  Replace the batteries.
>     - Error classification: Remote error
> * *Image is fuzzy or distorted (I)* - If your television shows a fuzzy or distorted image then your aerial socket has snapped off.  Insert a metal fork or thin conductive object into the socket.
>     - Error classification: TV Error
> * *Image is fuzzy or distorted (II)* - If your television shows a fuzzy or distorted image then your aerial has no reception.  Climb onto your roof and wiggle the aerial until the image improves.
>     - Error classification: Environment error
>
> Before attempting to solve any TV errors you should give your television a sharp blow to the top of the set.
> Before attempting to solve any remote errors you should throw the remote control at a wall.
> Before attempting to solve any environment errors you should throw a lightly salted potato chip over your left shoulder.

## Milestones

1. Create custom error objects to represent each of the different types things which can go wrong with your TV.  The error object should inherit from objects which represent the "Error classifications", which should themselves inherit from the `Error` object.  If you are unsure of how to create custom error types, take a look at the [MDN documentation for the `Error` object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error).
2. Update the `turnOn`, `switchChannel`, and `watch` methods of [the API](gist) to use your error objects, and run the callback or errback methods as appropriate.  For more information on callbacks take a look at [this assignment on the callback pattern](https://courses.thinkful.com/node-001v4/assignment/4.2.2).
3. Write a small test application which tries to turn on the TV, switch channels, and then watch the TV.  If any of the stages fail then you should call the function which attempts the fix described in the manual, then retry the stage.

## Additional Resources

* For a more complete look at JavaScript inheritance, take a look at [this chapter](OOJS - Chapter 6)
* [This article](http://thenodeway.io/posts/understanding-error-first-callbacks) describes some of the design rationale behind error-first callback, and gives examples of how they can be user.

## Example Solution

[To come]

