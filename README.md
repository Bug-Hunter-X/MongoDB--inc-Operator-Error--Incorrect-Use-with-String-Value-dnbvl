# MongoDB $inc Operator Error: Incorrect Use with String Value

This repository demonstrates an error that can occur when using MongoDB's `$inc` operator incorrectly. The `$inc` operator is used to increment a numeric field in a document. However, if you provide it with a string value, it will not function as expected, and might even corrupt your data.

## Bug

The `bug.js` file shows an example of incorrect usage of the `$inc` operator.  The code attempts to increment the `counter` field with the string value "1".

## Solution

The `bugSolution.js` file shows the corrected code.  The string value is now properly replaced with a number to ensure correct functionality. 

## How to reproduce the bug

1.  Set up a MongoDB database and collection. 
2. Insert a document with a numeric counter field e.g., `{"counter": 0}`
3. Run the code in `bug.js`. Observe the unexpected result.
4. Run the code in `bugSolution.js`. Observe the correct increment.
