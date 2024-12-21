# Unexpected Behavior in Ruby Due to Dynamic Typing

This repository demonstrates a common type-related issue in Ruby that can cause unexpected behavior and runtime errors. Ruby's dynamic typing provides flexibility but can lead to difficulties when dealing with type-related errors, as the code may not exhibit these problems until runtime.

## Bug Description
The `bug.rb` file contains a simple class `MyClass` with a setter and getter for an instance variable `@value`. While the setter method lacks type checking, it accepts values of different types, even though it's intended for integers.

## How to Reproduce
1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `ruby bug.rb`.
4. Observe that the program accepts string assignments to an integer-intended instance variable without any immediate errors.

## Solution
The `bugSolution.rb` file demonstrates a solution to mitigate this problem using type checking or more robust input validation in the setter method.

## Additional Notes
This example highlights the importance of careful type handling in Ruby, especially when dealing with code that interacts with external data or user input. Although Ruby's dynamic nature is beneficial, it requires extra vigilance to avoid type-related errors.
