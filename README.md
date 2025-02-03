# JavaScript Null Handling Bug

This repository demonstrates a common yet subtle bug in JavaScript related to null value handling during arithmetic operations.

The `bug.js` file contains the faulty code.  The `bugSolution.js` file offers a corrected version.

The bug arises from the implicit type coercion of JavaScript. When attempting to add a number and `null`, the `null` value is treated as `0`, resulting in unexpected behavior. The solution involves explicitly checking for `null` values and handling them appropriately. 

## How to Reproduce

1. Clone this repository.
2. Run `bug.js` using a JavaScript interpreter (Node.js, for example).
3. Observe the unexpected output for `foo(null, 1)` and `foo(1, null)`.
4. Run `bugSolution.js` to see the corrected output.

## Solution

The solution involves explicit null checks and handling within the function. This ensures more robust and predictable behavior in such cases.