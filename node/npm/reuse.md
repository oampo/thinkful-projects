title:                  Power Pack: Packaging with npm  
description:            Publish and use your own npm packages.  
duration:               4 hours  
skill_level:            Intermediate  
core_concepts:          installing npm packages, creating npm packages, sinopia  
prerequisite_concepts:  command line, JavaScript, JSON, Git, GitHub  

slug:                   reuse  
tags:                   Node  
date_implemented:       June 24, 2014  


## Project Brief

You just started as the first full stack developer at Initech, a mission-driven company billed as "Uber for Financial Services Consulting". Over the last two years of proving product-market fit they've built a monolitic Python application. Now they're ready to scale and your job is to convert to a microservices architecture.

As you review a 5,004 line legacy `user/models.py` file your eyes glaze over and you find yourself daydreaming about code reuse, comprehensible modules and, well, JavaScripting all the things.

Several of your microservices will need to reuse the same code, so for this project you'll create and publish your internal common libraries as Node packages to [sinopi](https://blog.dylants.com/2014/05/10/creating-a-private-npm-registry-with-sinopia/), a private Node registry.

## Milestones

### Milestone 1: Up and Running with Node and npm

If you haven’t used npm before, you should learn what npm is, how to install and update it, fix permissions, and install existing npm packages. Work through Section 1 through Section 4 of the [“Getting Started”](https://docs.npmjs.com/) guide in npm’s docs.

### Milestone 2: Installing Existing Packages

[To come]

[Should include global installation of [How to npm](https://github.com/npm/how-to-npm), a package that helps you package. Perhaps other packages?]

### Milestone 3: Creating and Publishing New Packages

[To come]

[Create two packages.  Package2 should include Package1 using [npm link](https://docs.npmjs.com/cli/link).]

[Should we use a stripped-down version of the tfcommons package to provide a sample package if they don't want to build their own?]

[Publish your packages to a private registry with [sinopia](https://blog.dylants.com/2014/05/10/creating-a-private-npm-registry-with-sinopia/)]

##Additional Resources

* If you are worried that your dependency's dependencies are going to cause issues, you can force them to remain the same version.  Lock down max's dependencies with [shrinkwrap](https://docs.npmjs.com/cli/shrinkwrap).
* [Node module lookup](https://nodejs.org/api/modules.html#modules_loading_from_node_modules_folders)
* [More resources to come]
