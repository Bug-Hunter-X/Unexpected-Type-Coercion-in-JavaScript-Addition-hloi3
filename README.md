# Unexpected Type Coercion in JavaScript Addition

This repository demonstrates a common JavaScript bug caused by loose typing and implicit type coercion in the addition operator (+).

## The Bug
The `foo` function aims to handle null values gracefully. However, the addition operation doesn't behave as expected when one operand is a number and the other is a string. JavaScript implicitly converts the string to a number, which can lead to incorrect results, or, in this case, concatenation.

## The Solution
The improved `foo` function explicitly checks the types of the inputs and performs addition only if both values are numbers. If either value is null or not a number, it returns 0. This prevents unexpected type coercion and ensures the function behaves as intended.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` to see the buggy code.
3. Open `bugSolution.js` to see the corrected code.
4. Run each JavaScript file using Node.js or a similar JavaScript runtime.