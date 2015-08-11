Following the runaway success of [Pride and Prejudice and Zombies](https://en.wikipedia.org/wiki/Pride_and_Prejudice_and_Zombies), you have decided it's the perfect time to get into the publishing game.  So in the space of ten minutes you've produced a first draft of "Pride and Prejudice and Velociraptors", using this piece of CLI magic:

```
sed 's/\(\(Mr\|Mrs\)\.\|\(Miss\|Sir\|Lady\)\)/Velociraptor/g' input.txt > output.txt
```

Eagle-eyed readers may spot what Random House did not: all that the command does is replace the strings Mr., Mrs., Miss., Sir, and Lady with the string Velociraptor.

To help speed up the production of your future manuscripts you have decided it is time to implement a build system to automate away the difficulties of creating such groundbreaking writing.

## Milestones

### Milestone 1: Add the Velociraptors

In this milestone you are going to use NPM to set up a basic build system to produce Pride and Prejudice and Velociraptors from the original source material.

To complete the milestone you should.

* Create a new project, and `npm init` it.
* Add `src` and `build` directories to the project.
* Download a .txt copy of Pride and Prejudice from [Project Gutenberg](http://www.gutenberg.org/cache/epub/1342/pg1342.txt), and add it to the `src` directory.
* Create a `build` task in the `scripts` section of `package.json`, which runs the `sed` command on the text file and puts the output into the `build` directory.
    - Notice that you will need to escape the backslashes with a second backslash to make them valid JSON

Try running your build command using `npm run build`, and take a look at the output to make sure that it has worked correctly.

#### Sample Code

When you have completed the milestone, take a look at [this sample `package.json` file](https://gist.github.com/oampo/ee167ff8f846a1d864fd).

### Milestone 2: Add some extra utilities

In this milestone you are going to add some extra utility tasks to help with the book creation progress.  To complete the milestone you should add the following tasks:

* `mkdir` - Should create the build directory, failing silently if the directory already exists.  This should also be run before the build task if `npm run build` is called.
* `read` - Should use `less` to allow you to read the built file.
* `read-src` - Should use `less` to allow you to read the original file.
* `clean` - Should delete the build directory.

#### Sample Code

When you have completed the milestone, take a look at [this sample `package.json` file](https://gist.github.com/oampo/e4e53aac3acab13be053).



