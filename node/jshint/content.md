Signor Daniele Omino, the famous Italian pizzeria impresario, is a perfectionist.  He likes his pizzas precisely 3mm thick.  He likes exactly 21g of mozzaralla on his margherita.  And he likes his order processing code to be beautifully written.  So you can only imagine his horror when a contractor presented him with [this code]().  It works, but it sure ain't pretty.

The contractor was fired on the spot, and you were hired to clean up the mess.  And Signor Omino made it clear that if you can demonstrate to him that you take as much care over your code as he does his pizza, then you can have the job full-time.

# Resources

* [This article](http://www.smashingmagazine.com/2015/02/avoid-javascript-mistakes-with-static-code-analyzer/) provides an introduction to the use of static code analysis tools to check the quality of your JavaScript code.  It includes a section on JSHint, the tool which you will be using in this project.
* The list of [JSHint options](http://jshint.com/docs/options/) provides context about when errors are thrown by JSHint, and how they can be fixed.

# Milestones

## Milestone 1: Clean up the code

In order to get paid for the contract you need to fix up the code from the previous contractor.  To complete this milestone you should:

* Install [JSHint](http://jshint.com), using `npm install -g jshint`.
* Download the code from [this gist].
* Tell JSHint to enforce all of its rules, by adding the following comment to the top of the file: `/* jshint enforceall:true */ `.
* Run jshint on the file: `jshint pizza-order.js`.
* Fix the errors one-by-one, until you are down to zero errors.

## Milestone 2: Set your house in order

In order for S. Omino to hired you on a full-time basis you need to demonstrate that at least two more codebases pass the JSHint test.  So pick two earlier projects which you have worked on, and run JSHint on all of the code, fixing any errors which you find.

