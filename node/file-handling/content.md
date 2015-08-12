Messrs [Rivest, Shamir, and Adleman](https://en.wikipedia.org/wiki/RSA_%28cryptosystem%29) have been at it again.  And this time they've come up with something really special.  A 100% secure, uncrackable two-way encryption algorithm for plain text in only [36 lines of JavaScript](https://gist.github.com/oampo/e1ff775c04e79e1385d8).

While they rest on their laurels, you have been tasked with packaging their algorithm into an easy-to-use app which will read an input file and either encode or decode it, writing the output into a second file.

## Milestones

### Milestone 1: Do it in sync

To complete this milestone you should write a script which uses the synchronous versions of the `fs` file handling functions to read in a file, transcode it using the `transcode` function [from `rsa13.js`](https://gist.github.com/oampo/e1ff775c04e79e1385d8), and output it to a new file.  The filename should be provided as command line arguments.

Test out your program by running a simple text file through the transcoder to encode it, and take a look at the output.  You should see some heavily encrypted nonsense.  Then try running your encrypted file back through the transcoder.  You should get your original message back.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/f84acfdb4ab7c003a362).

### Milestone 2: Make it async

In time your code might be used to encode multiple files in parallel.  So to complete this milestone you should update your code to use the async versions of the `fs` methods.

#### Sample Code

When you have completed this milestone, compare your code with [this sample](https://gist.github.com/oampo/5a878d420fa954e7415a).

## Important Note

Please don't _actually_ use this algorithm to encrypt your sensitive data.  Read the code carefully if you want to know why.


