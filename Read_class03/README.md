# Read class03 : FileIO & Exceptions

### What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

* The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error and makes handling any unexpected errors easier for you.
---------------

### Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method

* .read()	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.
* .readline()	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.


for example :
- file contains this :

```text
Hello, I am Tala !
This is Read class03.
I'm learning python in LTUC
```
```
read()' reads the entire file into a single string and the output will be as is :

Hello, I am Tala !
This is Read class03.
I'm learning python in LTUC

But readline(5) reads each line of the file one by one.
the output will be

Hello,
 I am
  Tal
  a !
This 
is Re
ad cl
ass03
.
I'm l
earni
ng py
thon 
in LT
UC

```

--------------------------

### Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example

is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions

* A try clause is executed up until the point where the first exception is encountered.
* Inside the except clause, or the exception handler, you determine how the program responds to the exception

* finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions

example : 
```python
try:
    linux_interaction()
except AssertionError as error:
    print(error)
finally:
    print('Cleaning up, irrespective of any exception')
 ```