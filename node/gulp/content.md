[Bonsai Kitten](https://en.wikipedia.org/wiki/Bonsai_Kitten), the infamous miniature kitten emporium, have just received their hosting bill and it is astronomical.  It probably has something to do with the hundreds of cat GIFs which they are using for advertising purposes.  To fix the problem Bonzai Kitten's owner, Dr Michael Wong Chang, instructs you to set up a system for minifying the images.  That's right: as well as compressing cats, you are now in the business of compressing cat GIFs.

Given that the collection of promotional GIFs is getting larger by the day, you decide that it's time to set up a build system using [Gulp](http://gulpjs.com/), the streaming build system.

## Milestones

### Milestone 1: A build task

To complete this milestone you should clone the GIFs from [this repository](https://github.com/oampo/bonzai-kitten-gifs).  Next set up a gulpfile which contains a task to compress the GIFs.  The task should use the [gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin) and [gulp-changed](https://www.npmjs.com/package/gulp-changed) plugins to compress the images, adding the compressed files to the `build` directory.

To check that your task is working, run your Gulp task, and compare the sizes of the compressed and uncompressed GIFs.

#### Sample Code

When you have completed this milestone, take a look at [this sample gulpfile](https://gist.github.com/oampo/9f9997e73ec4133de05a).

### Milestone 2: A clean task

Often when you have a build system set up you want to completely clear the previous build so you can re-run the build from scratch.  To complete this milestone you should set up a `clean` task, which deletes all of the files in the `build` directory using the [del library](https://www.npmjs.com/package/del).  Note that the `del` function is asynchronous, so you will need to set up your Gulp task accordingly.

#### Sample Code

When you have completed this milestone, take a look at [this sample gulpfile](https://gist.github.com/oampo/aa373b10f46f1101c836).

### Milestone 3: A watch task

To complete this milestone, you should set up a `watch` task for the GIFs.  Whenever you add or change one of the images this should run the build task.  The `watch` task should have the `build` task as a prerequisite, so that when you run `gulp watch` your images will be in a compressed state to start with.

#### Sample Code

When you have completed this milestone, take a look at [this sample gulpfile](https://gist.github.com/oampo/14c66b4b6d8515a34f3d).


