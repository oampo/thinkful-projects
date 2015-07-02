title:                  _cat_ pictures
description:            Use node.js streams to build common utilities.
duration:               4 hours
skill_level:            Advanced
core_concepts:          streams, pipes
prerequisite_concepts:  javascript, UNIX command line 

tags:                   
date_implemented:       
slug:                   

## Project Brief

Going back to the earliest versions of UNIX, ancestor to LINUX and OS/X, programmers have used powerful abstractions called _streams_ and _pipes_.

In this project, you'll see how node.js provides these same abstractions, by using them to implement simple versions of the _cat_ and _wc_ commands.


## Steps

Milestone 1: Build a simple _cat_ command using streams.

1. Create a Node script `cat.js` that uses streams to copy a file on `stdin` to `stdout`.  Create a test file named `my_text_file.txt` containing several lines of amusing text (you can copy (these)[http://www.azlyrics.com/lyrics/djjazzyjeffthefreshprince/freshprinceofbelairthemesong.html] if you're short on time). Refer back to the tutorial above if you get stuck.

2. Test by running

```sh
$ node cat.js < my_test_file.txt
```

You should see the contents of your `my_test_file.txt` output to your terminal window.

Milestone 2: Build a _num_ command that adds line numbers ahead of each line in a text file.

Remember that the data in a Node stream is just raw bytes. In order to interpret it as lines, you need to add a _codec_ into your stream when you create it.

1. Create a node script `num.js`, such that when given a file that looks like:

```
For he's a jolly good fellow,
for he's a jolly good fellow
```

The output should look like:


```
1: For he's a jolly good fellow,
2: for he's a jolly good fellow
```

2. Test by running

```sh
$ node num.js < my_test_file.txt
```

Milestone 3: Implement a simple version of the _wc(1)_ command using Node streams.

1. Create a Node script `wc.js` that prints the number of lines, words, and characters. So, for example,

```sh
$ node wc.js < my_test_file.txt
42 316 1581
```

(assuming, of course, that your file _has_ 42 lines, 316 words, and 1581 characters.)

2. Test by comparing the output of the real _wc(1)_ command to your Node script.


## Resources

1. This [useful tutorial](http://howtonode.org/coding-challenges-with-streams) explains the basics of using streams.
