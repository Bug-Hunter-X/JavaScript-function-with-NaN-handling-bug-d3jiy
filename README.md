# JavaScript Function with NaN Handling Bug

This repository demonstrates a common yet subtle bug in JavaScript related to handling NaN (Not a Number) values within functions.

The `bug.js` file contains a JavaScript function that intends to add two numbers. It correctly handles `null` values. However, if either input is `NaN`, the function will return `NaN`, which might not always be the desired behavior.

The solution is provided in `bugSolution.js` which addresses the NaN issue directly.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and examine the function `foo`.
3. Run `bug.js` using a JavaScript environment (Node.js or browser console).
4. Observe the output; you'll see that it returns `NaN` when one of the input is `NaN`, which is unexpected.

## Solution

The solution is implemented in `bugSolution.js`.  It explicitly checks for `isNaN` before performing the addition. This ensures that the function handles NaN inputs more robustly.