## Building Awesome Projects

Thinkful projects teach students core concepts or tools through practice.  Projects *aren't* tutorials or walkthroughs. Their purpose is to get the student to practice a real-world skill through an activity or exercise. The project itself should be a clear, actionable roadmap that fills in knowledge gaps when necessary by linking to external content. These guidelines will help you design an awesome project.

Each project hones in on just a few core concepts and requires the student to learn and implement those concepts.  As you begin to create your own project brief, ask yourself these questions:

- "What core concepts do you want to teach?"

- "What prerequisite knowledge does the student need to learn those core concepts?"

- "What real-world projects and tasks require an understanding of these core concepts?"

Get a taste for awesome projects with these examples:

- Building your first [Node server](https://projects.thinkful.com/12) with Node and Express to greet Jedi.

- Fixing a [leaky application](https://projects.thinkful.com/15) to understand memory leaks and profiling by.

- Building a [social network](https://projects.thinkful.com/7) to practice authentication and routing.

Create your project using the shiny new [Project Editor](projects.thinkful.com).

### Metadata

Each project brief requires the following [metadata](http://hiltmon.com/blog/2012/06/18/markdown-metadata/) fields at the top of the file:

- **Title**: The title of your project. Your title should be engaging and descriptive.  It should communicate (1) your core concepts and (2) what kind of project the student will build.
For example, the title "[OKCoding: Functional Programming with Lodash](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/lodash/dating.md)" includes core concepts (Lodash, functional programming) and a hint about the project ("OKCoding", a play on dating apps).

- **Description**: A one to three sentence description of your project. This is what users will read when deciding whether to start working on your project. For example, the [OKCoding: Functional Programming with Lodash](https://projects.thinkful.com/14) description is: "Use some of the most common Lodash methods to solve complex problems with simple code. This series of exercises will get you comfortable with the library and show off its strengths." If you chose your project from the [topics.md file](https://github.com/Thinkful-Ed/thinkful-projects/blob/master/node/topics.md) you can simply plug in the description from there.

- **Duration**: A time estimate for reading any essential content you link to and completing the project.  In general, simpler, more concise projects in the 2 - 3 hour range are better than complex projects that a student would complete over multiple days.

- **Skill Level**: In a general topic area (like Node, Angular, or React) projects should be aimed at students who are beginners, intermediate, or advanced in that topic area.

- **Core Concepts**: The one to three core concepts your project covers. You should expect students working on your project have little to no familiarity with these concepts, particularly with beginner level projects.

- **Prerequisite Concepts**: The concepts students need to understand before starting your project. You'll assume students have at least an intermediate level understanding of these topics or brush up on them in advance. If your prerequisite concepts are difficult or complex it's a good idea to link to refresher content in the 'Resources' section below.


### Project Brief

Your project brief sets the stage for the student. Have fun with the scenario. Maybe the student should imagine they are [working for NASA](https://projects.thinkful.com/10) to solve problems in space. Or maybe they're working for Google to serve you more ads. You should provide realistic context with a tangible outcome in a way that's fun to read. This is your chance to be creative.

The brief should also explain precisely what the final product does. If there's a visual output, show an example of what it could look like; if not describe the functionality in clear terms, such as ["visiting /jedi/Beyonce/Knowles should respond with ‘Hello KnoBe.'"](https://projects.thinkful.com/12).  By the time students finish reading this section the end goal of the project should be clear.

### Resources

Get students kickstarted by providing useful resources. This section should cover topics the student might want to research during the project and link to authoritative content for each topic.

For example, a project like [Tracking Down Memory Leaks in Node Apps](https://projects.thinkful.com/15) includes a book chapter on references in JavaScript, an article on Node modules for detecting memory leaks, documentation on memory profiling in Chrome, and a postmortem article from Netflix on chasing down memory leaks in their own Node app. Each resource should have one to three sentences explaining *what* the resource is and *why* it's useful.

When linking to resources, you can link to Thinkful course content, content we've licensed (see this [list](https://docs.google.com/spreadsheets/d/1Zgx5ObMFN3Xl8Q3ZozLvfz6SN-yPXjvnmt4FGEnn2ts/edit#gid=0) of available content), official documentation, or resources from around the web like high quality blog posts and articles.  Use the most appropriate content possible, but keep in mind that content we've developed or licensed is generally preferred as we can guarantee quality and reliability.

### Milestones

Break your project down into realistic and discrete "Milestones."  Give each milestone a short title, like: "Milestone 1: Build your Server and Get it Running" or "Milestone 2: Greet the Jedi".

Give clear steps or requirements to implement for each milestone. Use separate paragraphs or a list for clear structure. Beginner level projects should include specific, precise steps.  Advanced projects should have general steps that encompass several related tasks at once.

For each step, link to content that explains the concepts, tools, or skills the student needs to complete that step.  For example, you could close a milestone with language like: "if you need help with either step, review [Simple Express servers and Request parameters](https://courses.thinkful.com/node-001v4/assignment/2.1.1)."

Students should be able to complete individual milestones in a single sitting. Your first milestone, in particular, should take half an hour or less to complete. Big, complex initial milestones are a sign that the project is overly complex or too difficult for students to begin.

You can increase the difficulty of a project by adding bonus milestones. This helps keep the core project simple and is a great way for students to personalize their project or explore related concepts.  See [Space Jam: Save NASA Using External API's](https://projects.thinkful.com/10) for a great example of layering complexity with bonus milestones.


### Example Solution

Finally, provide a link to a reference solution to your project, ideally on GitHub.  That's it!

### Next Steps

After your initial draft, take a pass over your project and ask yourself the following questions:

 - Reread the "Core Concepts" you wrote down. Does your project focus clearly on these concepts?

 - Reread the "Prerequisite Concepts" you wrote down.  Do you need to add or remove any concepts now that you have your project brief and milestones?

 - Reread your project's "Description".  Is it still accurate?  Do you want to revise the description to match the project or tweak your project to match your original description?

 - Review your "Project Brief". Is it fun to read, and does it show personality? Does it give the student the context they need to understand why they're implementing your core concepts?

 - Review your "Milestones".  Can a student complete the first milestone in 30 minutes or less?  Is each milestone clear and discrete?  Is there any room for the student to customize the project and make it their own?

 - Review the "Resources" you link to. Did you cover gaps students might need to fill in their knowledge?  What about common pitfalls? Are there any terms you expect they'll google that you didn't include a resource for?

Once you've answered these questions for yourself you're ready for feedback on your project. Slack Zoe (@zoe) or Grae (@grae) with any questions.
