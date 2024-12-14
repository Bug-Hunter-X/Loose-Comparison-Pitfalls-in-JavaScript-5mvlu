# Loose Comparison Pitfalls in JavaScript

This repository demonstrates a common JavaScript error involving loose comparison (==) with null and undefined.  The example showcases unexpected behavior when checking for null specifically, while also inadvertently handling undefined and 0.

## The Bug
The `foo` function intends to return 0 only when the input `x` is strictly null. However, due to the use of loose comparison (==), it also returns 0 for `undefined` and 0, resulting in unintended behavior.

## The Solution
The recommended approach is to use strict equality (===) to avoid this issue and ensure that only null is treated as the special case.

## How to Run

1. Clone the repository.
2. Open `bug.js` to see the original buggy code.
3. Open `bugSolution.js` to see the corrected version.
4. Run the JavaScript files using a node interpreter (node bug.js or node bugSolution.js) to observe the output.