# Type Error in TypeScript Addition Function

This repository demonstrates a common type error in TypeScript where an explicit type annotation does not match the actual runtime behavior.  The function `add` is explicitly typed to accept two numbers, but the code calls it with a number and a string.

## Bug

The `bug.ts` file contains the erroneous code.  TypeScript will successfully compile this, however the runtime behavior will be unexpected.   The incorrect type annotation allows a string to be passed as an argument, leading to string concatenation instead of numerical addition. 

## Solution

The `bugSolution.ts` file demonstrates how to solve this issue. We use Type Guards to improve type safety.