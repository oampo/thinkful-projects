Level: Beginner

Time: 2 hours

Goals: Write your first program using Node streams, implementing simple versions of the *NIX `cat` and `wc` commands.

Concepts: Node, streams, pipes, codecs

Pre-reqs: Proficient with JavaScript, confortable with the command line

## Project

Going back to the earliest versions of UNIX, ancestor to LINUX and OS/X, programmers have used powerful abstractions called _streams_ and _pipes_.  The idea was simple: treat all data as a sequence of bytes, and pass them through programs that make some change in the sequence of bytes, and then emit them in a way that makes those bytes available for another program. So, for example, you might write this shell command:

```sh
$ cat < myfile.txt > newfile.txt
```

The _cat(1)_ command copies everything on `stdin` to `stdout`, and the redirection characters `<` and `>` connect named files to `stdin` and `stdout`. (In fact, in the very earliest UNIX systems, files were copied using this idiot; the _cp(1)_ command came later.)

A _pipe_ connects the output of the program on its left hand side to the input of a program on its right hand side.  So, a UNIX user might write:

```sh
$ cat < myfile.txt | wc
```

using the _cat(1)_ command to copy its file to `stdout`, where it is "piped" to `stdin` for the _wc(1)_ command, which then counts the number of lines, words, and characters and prints the results.

This apparently simple notion of streams and pipes turns out to be a powerful abstraction. Node has a built-in abstraction called a stream which is used to abstract a variety of input and output – for example, data arriving from the Internet over HTTP – into this simple stream and pipe model.

In this project, we will use Node's streams and pipes to implement simple versions of the _cat_ and _wc_ commands.

This [useful tutorial](http://howtonode.org/coding-challenges-with-streams) explains the basics of using streams; review it before beginning these milestones if you're new to streams.

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

1. Create a Node scripe `wc.js` that prints the number of lines, words, and characters. So, for example,

```sh
$ node wc.js < my_test_file.txt
42 316 1581
```

(assuming, of course, that your file _has_ 42 lines, 316 words, and 1581 characters.)

2. Test by comparing the output of the real _wc(1)_ command to your Node script.

