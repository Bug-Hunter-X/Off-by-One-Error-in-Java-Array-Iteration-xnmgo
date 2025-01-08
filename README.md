# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java code that occurs when iterating over arrays. The error leads to an `ArrayIndexOutOfBoundsException`.

## Bug Description

The `bug.java` file contains a for loop that iterates from 0 to `array.length`, inclusive.  This is incorrect because array indices start at 0 and end at `array.length - 1`. Accessing `array[array.length]` results in an `ArrayIndexOutOfBoundsException`.

## Solution

The `bugSolution.java` file shows the corrected code. The for loop condition is changed to `i < array.length` to prevent the out-of-bounds access.

## How to reproduce the bug

1. Compile `bug.java`: `javac bug.java`
2. Run `bug.java`: `java MyClass`

You will see an `ArrayIndexOutOfBoundsException`.
