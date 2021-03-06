Level: Intermediate

Time: 45 minutes

Goals: Find the memory leaks in a bidirectional-map implementation

Concepts: Memory leaks, profiling

Pre-reqs: Proficient with JavaScript.  Understanding of how garbage is collected in JavaScript.

# Project brief

It's your first day at your new programming job at the infamous CIA bothering shop WikiLeaks.  While Julian Assange has been busy [eating Ferrero Rocher](https://www.youtube.com/watch?v=4P-nZZkQqTc), it seems that coding standards have slipped.  Your new boss calls you over, and explains that hashing is vital to secrecy at WikiLeaks, and that to help the effort he's been working on implementing a bidirectional map(*).  Before running off for a long, boozy lunch he asks you to take a look over the code because it keeps running out of memory.

You take a look at the code, to find [this monstrosity](https://gist.github.com/oampo/da35215db9cd794c7aff).  All you have to do to keep your boss happy is to track down and fix the memory leaks.

# Milestones

1. Test out the code.  Try out the examples to make sure they work.  Try adding, removing, and filtering large groups of items whilst watching the memory usage.  Can you detect any leaks?  Does anything not work how you expected it to?  If you need some help understanding when memory might leak, have a read of the [MDN documentation on memory management](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management).
2. Take a read through the code, paying particular attention to any parts which seems unusual, or where you discovered leaky behavior in milestone 1.  Are there any obvious errors which would cause memory leaks?
3. Update the code to remove the memory leaks.  Although you might feel that a complete rewrite is in order (it definitely is!), think of your bosses feelings and try to keep the feel of the original code.

# Resources

* For a high-level recap of references in JavaScript take a look at [this chapter of JavaScript Allongé](https://github.com/Thinkful-Ed/js-allonge-book/blob/master/content/3_References%20and%20Rebinding/content.md)
* [This article](http://www.nearform.com/nodecrunch/self-detect-memory-leak-node/) introduces two Node.js modules which can be used to detect memory leaks in a Node application.
* The Chrome memory profiler can help you visualize how memory is being used in your application.  There is information about how to use the profiles, plus some useful information about how memory is stored and free in [this guide](https://developer.chrome.com/devtools/docs/javascript-memory-profiling)
* [This article from Netflix](http://techblog.netflix.com/2014/11/nodejs-in-flames.html) has a great account of finding an fixing a memory leak in a Node.js app.

# Footnotes

(*) Programmer Joke Alert: This one relies on you knowing that a [cryptographic hash function](https://en.wikipedia.org/wiki/Cryptographic_hash_function) is almost definitely a bad choice for implementing a Bidirectional Hashmap, a data-structure which has very little to do with secrecy and security.

