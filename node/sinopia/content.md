## Build

LennyCorp, developers of advanced facial recognition software, have a whole library of Node packages which they need to distribute to customers of their software.  To achieve this they have decided to set up a private NPM repository using [Sinopia](https://github.com/rlidwka/sinopia).

The first and most important module which needs publishing is [lenny.js](https://gist.github.com/oampo/72f81d1adacfcd2cf5b7), a simple module which contains [the Lenny Face](http://www.alexdantas.net/lenny/).  Used for everything from testing unicode compliance, to providing user feedback, the module is used in pretty much every piece of code which LennyCorp write.

## Milestones

### Milestone 1: Set up sinopia

To complete this milestone you should install sinopia as a global module, and run the `sinopia` command to start the server.  Then use `npm useradd` and add yourself as a user to the sinopia repository.

### Milestone 2: Publish `lenny.js`

Initialize a new project containing [the `lenny.js` file]().  Then use npm to publish the project to your private repository.  Make sure that you use the `--repository` flag so you don't accidentally publish the project to the public NPM repository.

### Milestone 3: Install from the repository

Create a new project and install the `lenny.js` module from your repository.  Then create a script which `require`s the module and logs the string.  Make sure that the module has been installed correctly by running the script.

