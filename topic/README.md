# Readings: Topic


### What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?

* Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes and You can create more than one object using a class.
* Classes are essentially a template to create your objects and You can declare class only once.	

* To create and manage instances of a class in Python, you can use the __init__ method, which is a special method that is called when an object is created from the class. This method can be used to initialize the object's properties, such as assigning values to instance variables.

----

### Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?

* A recursive function is a function defined in terms of itself via self-referential expressions
 * for example : Fibonacci number,factorial

* Python doesn’t have support for tail-call elimination. As a result, you can cause a stack overflow if you end up using more stack frames than the default call stack depth:

>>> import sys
>>> sys.getrecursionlimit()
3000

* Keep this limitation in mind if you have a program that requires deep recursion.
------
### What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.

* Fixtures define the steps and data that constitute the arrange phase of a test 
Code coverage measures the percentage of code lines that are executed by your tests and helps to identify untested code. Using pytest fixtures and code coverage together can reduce code duplication, ensure consistent test environments, increase test coverage, and identify untested code, ultimately improving the quality and maintainability of a Python project.
-----
## Things I want to know more about
nothig 