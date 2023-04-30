# Class 08 

### What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.

- Syntax : my_new_list = [ expression for item in list ]

|for loop|list comprehension|
|-|-|
|squares = []||
|for x in range(10): |squares = [x**2 for x in range(10)]|  
squares.append(x**2) ||

- it’s obvious that list comprehensions reduce the code necessary to complete rather complicated task when working with a list



### What is a decorator in Python?
-  decorator is a function that takes another function as input and extends its behavior without modifying its source code directly


### Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.
-To use a decorator, you simply apply the decorator function to the target function using the @ syntax or like this simple decorators exmaple:
```
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")

say_whee = my_decorator(say_whee)
```
the output :
```
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
```



## Things I want to know more about
read more about decorators 