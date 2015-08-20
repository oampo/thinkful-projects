## Build

[The 90s are back in fashion!](https://33.media.tumblr.com/2dfc3369827df9b981e111d7fd8fc732/tumblr_mvemcyarmn1rslphyo1_400.gif).  And to celebrate you've decided that it's time to bring back the `<blink>` and `<scroll>` tags.  But those pesky browser vendors have been out with the fun sponge and removed the tags.

Not one to be defeated easily, you've knocked up a couple of jQuery plugins which replicate the functionality.  But after months in Node-land you're wishing that you didn't have to go through all of the hassle of adding new `<script>` tags, and that you could just `require` the libraries and be done with it.  A five minute Google session turns up the [webpack](http://webpack.github.io/) module bundler.

## Milestones

### Milestone 1: Add the requires

To complete this milestone you should install webpack as a global module.  Then clone [this repository](https://github.com/oampo/blink-marquee) containing the `blink` and `marquee` plugins, plus an example of their usage.  Test it out by opening the `index.html` page.  Then add `require` tags to the scripts so that they can access their dependencies.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://github.com/oampo/blink-marquee/tree/m1).

### Milestone 2: Bundle it up

Use webpack to bundle the scripts, using `main.js` as your entry point.  Update `index.html` so it only sources your bundled JavaScript file.  Open up `index.html` in your browser.  You should see that the text is still blinking and marqueeing like it's 1999.


