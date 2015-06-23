Thinkful projects teach students core concepts or tools through practice and implementation.  Projects *aren't* tutorials or walkthroughs. Thinkful projects link to tutorial content to fill knowledge gaps, but their purpose is to simply present users with a clear, actionable roadmap for practicing real-world skills that results in a useful end product.

Each project hones in on just one or two core concepts and requires the student to learn and implement those concepts.  As you begin to create your own project brief, ask yourself these questions:
- "What core concepts do you want to teach?"
- "What prerequisite knowledge does the student need to learn those core concepts?"
- "What real-world projects require an understanding of these core concepts?"

Here are some examples of Thinkful projects:
- A beginner project on [building a web server with Node and Express](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/jedi.md).
- An intermediate project on [memory leaks in Node](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/memory_leaks/wiki-leaks.md).


Here is a project template for you to download and get started [***Note: we should link to a template markdown file here with appropriate metadata tags, headings, and empty lists.  The goal of that document should be to (1) standardize format and (2) reduce starting friction].  As you dig in, keep these guidelines in mind:


###Metadata
Each project brief requires the following metadata fields at the beginning of the file:
- Level: Beginner, Intermediate, or Advanced for the general topic area.  For example, setting up your first Node server is a beginner Node project, endpoint testing with Node, Mocha, and Chai (link) is an intermediate Node project, and XXXXX is an advanced Node project.
- Time Estimate: a time estimate for the project in minutes.
- Core Topics: the core topics you'll cover with this project
- Prerequisite topics: the topics the student needs to understand before they can get started on this project.

###Title
Your title should be engaging and descriptive. The project's core concepts should be clear from the title alone.
Here are some examples of good project titles:
- Garbage Collection with Node
- Your First Node Server
- Functional Programming with Lodash

###Project Brief
Your project brief sets the stage for the student. Have fun with the scenario for your project. Maybe the student should imagine they are working for NASA to solve problems in space. Or maybe they're working for Google to serve you more ads. You should provide realistic context with a tangible outcome in a way that's fun to read. This is your chance to be creative.

The brief should also explain precisely what the final product does. If there's a visual output, show an example of what it could look like; if not describe the functionality in clear terms, such as ["visiting /jedi/Beyonce/Knowles should respond with ‘Hello KnoBe.'"](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/first_node_server/jedi.md).  By the time they finish reading this section the end goal of the project should be clear to the student.

###Milestones
Break your project down into realistic "Milestones." At each "Milestone" the student should complete a discrete chunk of the project. For example, the title of your first milestone might be "Milestone 1: Build your Server and Get it Running", while the title of your second milestone might be "Milestone 2: Greet the Jedi".

Underneath the title, each milestone should have an ordered list of steps to complete.  Beginner level projects should include specific, precise steps.  Steps for advanced projects should be general and encompass several related tasks at once.

For each step, provide a link for the skills and concepts the student needs to complete that step.  For example, the last sentence of a step might read: "If you need help with either step, review [Simple Express servers and Request parameters](https://courses.thinkful.com/node-001v4/assignment/2.1.1)."

You can increase the difficulty of a project and touch on related topics by extending the basic project with "Bonus Milestones".  For each bonus milestone, include the words "Bonus Milestone" in the milestone title.  Check out the [Authentication and Routing in Node](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/authentication_and_routing/Thinkr.md) project for an example of how to extend projects like this.

### Resources
You should wrap up the project with an unordered list of useful resources that provide context and help for the student.  For example, a project like [Tracking Down Memory Leaks in Node Apps](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/memory_leaks/wiki-leaks.md) includes resources like: a book chapter on references in JavaScript, an article on Node modules for detecting memory leaks, documentation on memory profiling in Chrome, and a postmortem article from Netflix on chasing down memory leaks in their Node app. Each resource should have one to three sentences explaining *what* the resource is and *why* it's useful.

When linking to resources, you can link to Thinkful course content, content we've licensed (a list of available content can be found [here](https://docs.google.com/spreadsheets/d/1Zgx5ObMFN3Xl8Q3ZozLvfz6SN-yPXjvnmt4FGEnn2ts/edit#gid=0), official documentation, or resources from around the web like high quality blog posts and articles.  Use the most appropriate content possible, but keep in mind that content we've developed or licensed is generally preferred as we can guarantee quality and reliability.

###Sample Solution
Finally, provide a link to a reference solution to your project, ideally on Github.  That's it!

