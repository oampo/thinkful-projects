title:                  Lights Out: Using React  
description:            Build React components to control a set of lights.  
duration:               2 hours  
skill_level:            Intermediate  
core_concepts:          React, Click Handlers, Solvers (Advanced) 
prerequisite_concepts:  [To come]  

tags:                   React  
date_implemented:       June 30, 2015  
slug:                   lights-out-react 

You go over to your friend Jigsaw's house for a sleepover and after watching
Mean Girls twice, you decide it's time to hit the hay. When you get to the guest
bedroom, though, you discover that the entire ceiling is covered by a grid of lights!
Jigsaw says he's organized a game for you to play. To get to sleep, you have
to build a controller to turn off all the lights...but there's a catch. Every
time you turn a light on or off, the adjacent lights (the four lights above,
below, to the right, and to the left of the light you toggle) also get toggled.
You recognize this game as the [lights out game](https://en.wikipedia.org/wiki/Lights_Out_(game))
and decide to break out your coding skills so you can get some well-deserved rest.

Milestone 1:
  - Build a React component to represent a light that can be on or off
  - Build a React component to display a 5 by 5 grid of your light components on the screen
  - Write a click handler that Toggles a light on or off when you click it

Milestone 2:
  - Set the grid to have a random setting for the lights each time you start the game
  - Add to your click handler and toggle the adjacent lights when you press a light
  - Give yourself "props" by displaying an alert congratulating youself when all the lights are turned off

Bonus Milestone:
  - Make your grid scalable to any size > 0 by passing props into your grid component
  - Give your component some default props of 5 so you don't _have_ to pass anything in
  - Read up on [methods of solving lights out](http://www.logicgamesonline.com/lightsout/tutorial.html)
  - Guarantee yourself a good night's sleep and write a script to solve the lights out game.

Example Solution [here](http://codepen.io/ripleyaffect/pen/xGrByr)
