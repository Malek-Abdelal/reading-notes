# Class 04 Reading

## Classes and Objects

About the class, is a blueprint or a template that defines the structure and behavior of objects.

Also it provides a way to organize and encapsulate related data and functionality.

An object is an instance of a class. It represents a specific realization of the class, with its own set of values for attributes.

So each object created from a class can have its own unique data, independent of other objects of the same class.

---------- 

## Thinking Recursively

Recursion is a programming concept where a function calls itself to solve a problem by breaking it down into smaller, simpler instances of the same problem. It involves the process of solving a complex problem by solving smaller instances of the same problem until a base case is reached. The base case is a condition that determines when the function should stop calling itself and start returning values.

As an example of using recursion, we can create a function calculates the factorial of a given number 'n'.

When implementing recursive functions, it's important to follow these best practices: 

1. Ensure progress towards the base case: For a recursive function to work correctly, each recursive call should move the problem towards the base case. If the recursive calls don't reduce the problem size, the recursion won't terminate.

2. Define a base case: Ensure that your recursive function has a condition that determines when to stop the recursion. Without a base case, the function will continue calling itself indefinitely, causing a stack overflow error.

3. Optimize when possible: Recursive solutions can be inefficient for certain problems due to repeated function calls. Look for opportunities to optimize the recursion by using memoization (caching previously computed results) or employing techniques like tail recursion.

4. Use appropriate data structures: Sometimes, you may need to use additional data structures like lists or dictionaries to keep track of intermediate results or state during recursion.

So, By following these best practices, we can effectively use recursion to solve problems while avoiding common pitfalls and errors.

----------

## Things I want to know more about

So excited to learn more about OOP and going deeply in it.