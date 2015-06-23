title: Asynchronous Programming
description: Learn to avoid callback hell while processing a series of text files asynchronously. Use new features including promises, generators, and async.
duration: 
date_implemented: 
skill_level: Intermediate
slug:
tags: Node

##Brief

A noted ed-tech are rewriting the code which generates their curricula.  The curricula are stored on disk with the following structure:

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

The number of units, lessons, and assignments in each curriculum varies.  Your task is to read in each of the assignments and store them as a JavaScript object, for example:

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


##Caveats

* There may be other files in the curriculum directories.  Only files matching the `assignment-#.md` format should be added to the object.
* Some of the lessons may be symlinks to lessons from other curricula.  The symlinks should be followed to get to the content.
* The curricula may be very large, so in order to complete the task quickly the code needs to perform the IO asynchronously.

##Milestones

Milestone 1: Listing the file structure

1. Create a simple example directory structure without symlinks or extraneous files.
2. Write a function to list the contents of a single directory asynchronously.  You may need to revise the [Node fs module documentation](https://nodejs.org/api/fs.html), and look at [how to handle asynchronous programming without resorting to a tangle of callbacks](https://courses.thinkful.com/node-001v4/lesson/4.2).
3. Find out (asynchronously) whether any of the items in the directory are folders, and if they are, call your directory listing function recursively for each of them.

Milestone 2: Reading the assignments

Update your code to list in the content of the assignments.

Milestone 3: Creating the data structure

Update your code to build the required data structure as you walk through the directory tree.  You may need to revise the [methods for building objects and arrays](https://courses.thinkful.com/node-001v4/assignment/1.1.2).

Milestone 4: Handling the caveats

1. Add some extraneous files to your directory structure, and make one of the lessons symlink to a new directory.
2. Make sure your code handles these edge cases successfully.



