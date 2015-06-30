title:                  Asyncful: Asynchronous Programming  
description:            Learn to avoid callback hell while processing a series of text files asynchronously. Use new JavaScript features including promises, generators, and async.  
duration:               2 hours  
skill_level:            Intermediate  
core_concepts:          [To come]  
prerequisite_concepts:  [To come]  

tags:                   Node  
date_implemented:       June 23, 2015  
slug:                   asynchronous-programming  


##Project Brief

A noted ed-tech company is rewriting the application it uses to generate their course curricula.  The curricula are stored on disk with the following directory structure:

```
.
├── unit-1
│   ├── lesson-1
│   │   ├── assignment-1.md
│   │   └── assignment-2.md
│   └── lesson-2
│       ├── assignment-1.md
│       └── assignment-2.md
└── unit-2
    ├── lesson-1
    │   ├── assignment-1.md
    │   └── assignment-2.md
    └── lesson-2
        ├── assignment-1.md
        └── assignment-2.md
```

The number of units, lessons, and assignments in each curriculum varies.  Your task is to read each curriculum from disk and create a corresponding JavaScript object, for example:

```js
{
    units: [
        {
            lessons: [
                {
                    assignments: [
                        "Contents of U1L1A1",
                        "Contents of U1L1A2"
                    ]
                },
                {
                    assignments: [
                        "Contents of U1L2A1",
                        "Contents of U1L2A2"
                    ]
                }
            ]
        },
        {
            lessons: [
                {
                    assignments: [
                        "Contents of U2L1A1",
                        "Contents of U2L1A2"
                    ]
                },
                {
                    assignments: [
                        "Contents of U2L2A1",
                        "Contents of U2L2A2"
                    ]
                }
            ]
        }
    ]
}
```


###Caveats

* There may be other files in the curriculum directories.  Only files with titles matching the `assignment-#.md` format should be added to the object.
* Some of the lessons may be symlinks to lessons from other curricula.  The symlinks should be followed to get to the content.
* The curricula may be very large, so in order to complete the task quickly the code needs to perform the IO asynchronously.

##Milestones

### Milestone 1: Listing the file structure

1. Create a simple example directory structure without symlinks or extraneous files.
2. Write a function to list the contents of a single directory asynchronously.  You may need to revisit the [Node fs module documentation](https://nodejs.org/api/fs.html), and look at [how to handle asynchronous programming without resorting to a tangle of callbacks](https://courses.thinkful.com/tfl-001v1/lesson/4.2).
3. Find out (asynchronously) whether any of the items in the directory are folders. If they are, call your directory listing function recursively for each of them.

### Milestone 2: Reading the assignments

Update your code to list in the content of each assignment.

### Milestone 3: Creating the data structure

Update your code to build the required data structure as you walk through the directory tree.  You may need to revisit the [methods for building objects and arrays](https://courses.thinkful.com/tfl-001v1/assignment/1.1.2).

### Milestone 4: Handling the caveats

1. Add some extraneous files to your directory structure, and make one of the lessons symlink to a new directory.
2. Make sure your code handles these edge cases successfully.

## Resources

Need help getting started? Join the next frontend [Office Hours](https://open-sessions.thinkful.com/) or ask in the #front-end-web-dev channel on [Slack](https://thinkful-students.slack.com)

## Example Solution

Our solution is coming soon. Want us to take a look at yours? [Email us](dan@thinkful.com) a link to the GitHub project or share it on [Slack](https://thinkful-students.slack.com).
