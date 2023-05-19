# Class 08 Reading

## Ten Thousand 3

### Python list comprehension

The basic syntax of Python list comprehension follows this structure:

```python
[expression for item in iterable if condition]

```

Here's an explanation of each component:

- **expression:** This is the operation or computation you want to perform on each item in the iterable.
- **item:** It represents the individual elements in the iterable that you want to iterate over.
- **iterable:** It refers to the sequence, such as a list or a range, from which you want to create the new list.
- **condition** (optional): It allows you to include an additional filter or condition to control which items are included in the new list. This part is optional.

Now, let's compare list comprehension to using a for loop to create a list. When using a for loop, you typically initialize an empty list and then iterate over the elements in an iterable, performing an operation on each item, and appending the result to the list.

Here's an example that demonstrates the difference. Let's say we have a list of integers [1, 2, 3, 4, 5], and we want to square each element:

Using a for loop:

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = []
for num in numbers:
    squared_numbers.append(num**2)

```

Using list comprehension:

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = [num**2 for num in numbers]

```

As you can see, list comprehension allows you to create a new list and perform the squaring operation in a more concise and expressive way. It combines the iteration, operation, and appending steps into a single line. The resulting squared_numbers list will contain [1, 4, 9, 16, 25].

-----

### Decorators

In Python, decorators are a powerful feature that allows you to modify or enhance the behavior of functions or classes without directly modifying their source code. They provide a way to wrap or decorate functions or classes with additional functionality.

At their core, decorators are higher-order functions that take a function or class as input and return a new function or class. They can be used to add functionality, modify behavior, or provide additional features to the decorated object. Decorators are typically denoted using the '@decorator_name' syntax, placed just before the function or class definition.

Here's a simplified example to illustrate how decorators work:

```python
def decorator_function(original_function):
    def wrapper_function():
    
        print("Before the function is called")
        original_function()
        print("After the function is called")

    return wrapper_function

@decorator_function
def hello():
    print("Hello, world!")
hello()

```

In this example, we define a decorator function called '**decorator_function**'. It takes the original function ('**hello**') as input and returns a new function ('**wrapper_function**'). The '**wrapper_function**' is responsible for adding the additional behavior or actions before and after calling the original function.

When the '**hello()**' function is called, it is automatically decorated by the '**decorator_function**'. The output will be:

```sql
Before the function is called
Hello, world!
After the function is called

```

Common use cases for decorators include:

- **Logging**: Adding logging statements or tracking function calls.
- **Timing**: Measuring the execution time of functions.
- **Caching**: Storing and reusing function results to improve performance.
- **Authorization and authentication**: Checking user permissions before executing a function.
- **Error handling**: Catching exceptions and handling errors gracefully.

Decorators provide a clean and reusable way to extend or modify the behavior of functions or classes without modifying their original implementation, promoting code reusability and separation of concerns.