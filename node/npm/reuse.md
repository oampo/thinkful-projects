title:                  Power Pack: Packaging with npm  
description:            Publish and use your own npm packages.  
duration:               4 hours  
skill_level:            Intermediate  
core_concepts:          installing npm packages, creating npm packages, sinopia  
prerequisite_concepts:  command line, JavaScript, JSON, Git, GitHub  

slug:                   packaging-with-npm  
tags:                   Node  
date_implemented:       June 24, 2014  


## Project Brief

You have only been working as a full stack developer at Initech for two weeks, and you are already staging a coup.  Initech, a mission-driven company billed as "Uber for Financial Services Consulting", have spent two year proving product-market fit, during which time they've built a monolitic Python application.

As you review a 5,004 line legacy `user/models.py` file your eyes glaze over and you find yourself daydreaming about code reuse, comprehensible modules and, well, JavaScripting all the things.

You turn to your semi-comatose colleague in the adjacent cubicle and you tell her that together the two of you are making a stand.  There will be no more monolithic Python.  There will only be beautiful, modular JavaScript.

Your colleague shrugs her shoulders, takes a sip of Club Mate, and tells you that she has a bit of code laying around which you can use to convince the key stakeholder: your boss.

## Resources

* If you haven’t used npm before, read sections 1-4 of the [npm getting started guide](https://docs.npmjs.com/).  This will show you what npm is, how to install and update it, fix permissions, and install existing packages.
* The [how to npm module](https://github.com/npm/how-to-npm) is an interactive walkthrough of how to use various features of npm.
* If you are confused about where Node searches for modules which you install using npm, take a look at this documentation on [the Node module lookup order](https://nodejs.org/api/modules.html#modules_loading_from_node_modules_folders)
* For an introduction to sinopia
* [More resources to come]

## Milestones

### Milestone 1: Initialize the project and install the dependencies

Your colleague has written [a small utility in Node](https://gist.github.com/oampo/51c6c56d208f6d9ecea4) for adding new contractors to the database, and manipulating the ratings of contractors so everyone gets five-star service.

To complete this milestone you should:

* Create a new directory for the project
* Download [the code](https://gist.github.com/oampo/51c6c56d208f6d9ecea4) into the directory
* Initialize the project using `npm init`
* Use npm to install the project's dependencies, saving them to your `package.json` file.
* Have a read through of the utility, and try running the examples, so you understand how it works

### Milestone 2: Split out the database layer

To complete this milestone you should split your code into three separate projects: the database layer, and two separate utility applications for adding the contractors, and changing the ratings.

* The two utilities should use `npm link` to link to the database layer.
* You will need to add `module.export` and `require` calls to give you access to the database layer from the utilities.
* Each project should have its own `package.json` file listing the correct dependencies.

### Milestone 3: Publishing your packages

To complete this milestone you should set up [sinopia](https://github.com/rlidwka/sinopia) to act as a private registry.  You should then publish your three packages to the registry, and try installing them in a separate project to make sure that the registry is working correctly.


