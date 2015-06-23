title: npm
description: Publish and use your own npm packages.
duration: 4 hours
date_implemented: 
skill_level: Intermediate
slug:
tags: Node


Concepts: npm, package.json, sinopia
Pre-reqs: command line, JavaScript, JSON

##Project Brief

In order to reuse your code among all your projects, and allow others to use your code, you have to package your code in ...packages.  npm is the tool used to create and install packages into your application.  Once packages are installed, you can use the `require` function to include them in your code.  To get started with what npm has to offer, checkout [npm's screencasts](https://docs.npmjs.com/getting-started/what-is-npm) which teach you everything you need to know. 

##Milestones

* Create your own package called mini.
* Create a second project called max.  This time you want to require mini inside of max, but you can't publish mini or max to the npm registry (they're both taken).  Use [npm link](https://docs.npmjs.com/cli/link) to include mini inside of max.
* Now we want to create a private registry to host our max and mini packages.  [Using sinopia](https://blog.dylants.com/2014/05/10/creating-a-private-npm-registry-with-sinopia/) as your registry, publish max and mini.
* If you are worried that your dependency's dependencies are going to cause issues, you can force them to remain the same version.  Lock down max's dependencies with [shrinkwrap](https://docs.npmjs.com/cli/shrinkwrap).

##Additional Resources

* [How to npm](https://github.com/npm/how-to-npm)
* [Node module lookup](https://nodejs.org/api/modules.html#modules_loading_from_node_modules_folders)
