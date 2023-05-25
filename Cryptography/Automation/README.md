# Automation 

### How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary library to work with them?
- regular expressions are used to search for specific patterns within strings. The primary library for working with regular expressions in Python is the <re> module.
The re module provides various functions and methods to perform operations with regular expressions. The re.search() function is commonly used to search for a specific pattern within a string. It returns a match object if the pattern is found, or None if no match is found. Other functions like re.match() and re.findall() are also available for different matching scenarios 
### What is the purpose of the shutil library in Python, and provide an example of a common use case for file or directory management with this library?
- The shutil library in Python provides high-level operations for file and directory management. It offers functions for copying, moving, and deleting files and directories. Some of the commonly used functions in shutil include shutil.copy(), shutil.move(), and shutil.rmtree().

### Explain one automation idea from the assigned material and describe how it can be implemented using Python’s regular expressions and shutil libraries.
- One automation idea from the assigned material could be automating the backup of specific files or directories. This can be achieved using regular expressions to search for files or directories that match a specific pattern, and then using the shutil.copy() function to create backups.
