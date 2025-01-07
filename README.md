# JavaScript Loose Comparison Bug
This repository demonstrates a common but easily overlooked bug in JavaScript related to loose comparison using the == operator.

## The Bug
The function `foo` is intended to check if two values are equal. However, due to JavaScript's loose comparison, it can produce unexpected results when comparing different types.  For example, `foo(0, false)` returns `true`, even though 0 and false are distinct values.

## The Solution
The solution involves using the strict equality operator (===) to perform type-safe comparisons. This ensures that both the value and the type are matched before returning true.

## How to reproduce
1. Clone the repository.
2. Open `bug.js` and observe the function `foo`.
3. Open `bugSolution.js` and see the improved function `fooStrict`. 
4. Run tests in console to check the output. 