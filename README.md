# Unexpected Behavior When Directly Modifying Instance Variables in Ruby
This example demonstrates a potential issue in Ruby when directly modifying instance variables using `instance_variable_set` instead of using accessor methods (getters and setters). While this approach might seem convenient, it can lead to unexpected behavior and break the encapsulation principles of object-oriented programming.

## The Problem
In this code, we directly modify the `@value` instance variable using `instance_variable_set`. This bypasses any logic that might be within the `value` method, making it difficult to maintain and debug. This breaks encapsulation and can lead to inconsistent state changes that are hard to trace.

## The Solution
The recommended way to modify instance variables is through accessor methods.  This ensures that any validation, modification, or side-effects are correctly handled, enhancing code maintainability, readability, and predictability. 