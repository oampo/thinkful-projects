## Read & Watch

The Webhook CMS (which uses Swig for templating) provides a [screencast, and accompanying article](http://www.webhook.com/docs/template-inheritance-blocks/) on template inheritance which you should take a look at before getting started with this project.

## Build

Frank.en are a biotech startup who are planning to launch shortly, and are busy setting up a web presence.  They have a completed design for a two-page website, with plans to add further pages as they introduce new products.

The chief biologist, who is moonlighting as a web developer, is already tired of editing the HTML on two pages every time she wants to tweak the layout of the header.  You have been called in to help simplify her life using the magic of templates.

## Milestones

## Milestone 1: Up and running with Swig

In this milestone you will get the existing website code up and running, and start using Swig to render the HTML.

To complete the milestone you should:

* Clone the project from [this git repository](https://github.com/oampo/franken-template).
* Run the `index.js` file and visiting the site.  Try to get an idea of which sections you will be able to abstract away using template inheritance.
* Install Swig (`npm install --save swig`)
* Update the `index.js` script so that the HTML files are rendered using Swig, rather than using `res.sendFile`.  If you need a reminder on how to set up Swig with Express, take a look at [the Swig documentation](http://paularmstrong.github.io/swig/docs/#express)

#### Sample Code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/9a341ebc343657e8b0b5).

### Milestone 2: Split out a base template

To complete this milestone you should create a base template in the `views` directory called `base.html`.  This should include all of the elements which the two pages of the site have in common, along with `{% block %}` sections for the places where the pages diverge.  Don't forget, you can refer back to the [Swig documentation](http://paularmstrong.github.io/swig/docs/#inheritance) if you need to double check the syntax for inheritance.

To check your template, you can add a new endpoint to `index.js` which just renders the base template.

#### Sample Code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/753ddd915e891a372dab).


### Milestone 3: Extend the template

To complete this milestone you should update the two HTML pages so that they inherit from your newly created base template, overriding blocks where necessary.  Your final layout should look and work in the same way as the original pages, but with far less duplication of code.

#### Sample Code

When you have completed the milestone, take a look at [this sample code](https://gist.github.com/oampo/f9c67f94575a55a53182).

## Additional Resources

Some templating engines, such as Handlebars, don't support block-style inheritance.  Instead they use a system of partials to allow code reuse.  You can see how this pattern works in [the Handlebars documentation](http://handlebarsjs.com/partials.html).


