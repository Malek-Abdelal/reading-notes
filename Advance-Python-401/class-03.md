# class-03

## FileIO & Exceptions

**Q1** : What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

The 'with' statement in Python is used when working with resources that need to be managed, such as files. It provides a convenient way to ensure proper acquisition and release of resources, such as automatically closing files after their use. Here's the purpose of the 'with' statement when opening a file and how it helps manage resources:

1. **Automatic Resource Management:**
The primary purpose of the with statement is to ensure that resources are properly managed, even in the presence of exceptions or errors.

2. **Context Manager Protocol:**
The with statement is made possible by implementing the Context Manager Protocol. A context manager is an object that defines the __enter__() and __exit__() methods.

3. **Exception Handling:**
The with statement is particularly useful when handling exceptions. If an exception occurs within the with block, the __exit__() method is still called, allowing for proper cleanup and release of resources. 

- The 'with' statement provides a more concise and safer way to manage resources, such as files, in Python. It helps prevent resource leaks, simplifies exception handling, and promotes clean and robust code.

--------

**Q2** : Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python.

In Python, the 'read()' and 'readline()' methods are used to read data from a file object. However, they have different behaviors and are used in different scenarios. Here's the difference between 'read()' and 'readline()' methods and examples of when to use each method:

1. **'read()' Method:**
The 'read()' method is used to read a specified number of characters or the entire content of a file, depending on the parameter passed. It returns a string containing the read data.

- **Example:**

```
with open('file.txt', 'r') as file:
    content = file.read()
    print(content) 
```

**Use 'read()' when:**

- You want to read the entire content of a small file or a portion of a large file.
- You need the file's content as a whole, such as processing a configuration file or parsing a JSON file.

2. **'readline()' Method:**
The 'readline()' method is used to read a single line from a file. It returns a string containing the line, including the newline character at the end.

**- Example:**
``` 
with open('file.txt', 'r') as file:
    line = file.readline()
    while line:
        print(line)
        line = file.readline()
```

**Use 'readline()' when:**

- You want to process a file line by line, such as reading a log file or extracting specific data from a file.
- You need to iterate through a file sequentially, processing each line individually.

-------------

**Q3** : Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code?

Exception handling in Python is a mechanism that allows you to handle and manage errors and exceptions that may occur during program execution. Exceptions are unexpected events or conditions that disrupt the normal flow of code execution. Exception handling helps prevent program crashes and provides a way to gracefully handle errors.

The basic concept of exception handling involves the following elements:

1. **Exception:** An exception is an error or an exceptional condition that occurs during program execution.It can be caused by various factors, such as invalid input, division by zero, or file not found. Exceptions are represented by objects in Python and are instances of specific exception classes.

2. **Try-Except Block:** To handle exceptions, you enclose the code that might raise an exception within a try-except block. The try block contains the code that is potentially prone to exceptions. If an exception occurs within the try block, it is caught by the corresponding except block.

3. **Except Block:** The except block is where you define the code to handle specific types of exceptions. Each except block specifies the type of exception it can handle, allowing you to provide customized error handling logic for different types of exceptions. You can also have a general except block that catches any exception not handled by specific except blocks.

4. **Finally Block:** Additionally, you can include a finally block after the except block. The code within the finally block is executed regardless of whether an exception occurred or not. It is typically used to perform cleanup tasks or release resources, ensuring they are properly handled regardless of exceptions.

- **basic example of exception handling :**

``` 
try:
    result = 10 / 0  # Division by zero
except ZeroDivisionError:
    print("Error: Division by zero")
except Exception as e:
    print("An error occurred:", str(e))
finally:
    print("Cleanup tasks")
```