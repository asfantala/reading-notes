# Readings: Ten Thousand 2


## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both

* Global scope: The names that you define in this scope are available to all your code.

* Local scope: The names that you define in this scope are only available or visible to the code within the scope.
- for example
x = 10 --> global 

def my_func():
    y = 5 ->  y - local variable


## How do the global and nonlocal keywords work in Python, and in what situations might you use them?

Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function.

Global (or module)  This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.


## In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis

- the purpose of big O is to describe the performance of the algorithm and it is important it helps to analyze the efficiency of different algorithms

## Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials
- stimulate a dice roll using random.randint(1,6)
- Probability of rolling dice  = Number of desired outcomes ÷ Number of trials
- so we can use for loop to know number of desired outcomes by add +1 to count after finishing the loop divide the count over number of trials 