# MongoDB $inc operator error with string value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The `$inc` operator is used to increment a numeric field by a given value.  However, if a non-numeric value (such as a string) is provided, the update will fail.

The `bug.js` file contains the code that reproduces the error. The `bugSolution.js` file provides the correct implementation.

## How to reproduce the error

1.  Clone this repository.
2.  Ensure you have MongoDB installed and running.
3.  Run `bug.js` using Node.js. You'll see an error indicating that the `$inc` operator requires a numeric value.

## Solution

The solution is simple: ensure that the value you're incrementing with is a number, not a string. The `bugSolution.js` shows the correct usage of the `$inc` operator.