# README.md

## Read Assignment 7 TEN-THOUSAND 2

 Understanding variable scope, global and nonlocal keywords, Big O notation, and simulation of dice roll in Python are important  to writing effective and efficient code.

Variable scope refers to the accessibility of a variable within a program. Local scope variables are only accessible within a function or block of code, while global scope variables are accessible throughout the entire program. For example:

# Global variable
x = 10

def my_func():
    # Local variable
    y = 5
    print(x, y)

my_func()  # Output: 10 5
print(x)   # Output: 10
print(y)   # NameError: name 'y' is not defined

The global keyword is used to define a variable as global and make it accessible throughout the entire program, while the nonlocal keyword is used to access variables defined in a parent function. These keywords are useful when you want to modify global or nonlocal variables from within a function.

Big O notation is a mathematical concept used to describe the time complexity of an algorithm, which is the amount of time it takes to complete as the input size grows. It is important in algorithm analysis because it provides a way to compare the efficiency of different algorithms.

To simulate a dice roll in Python, you can use the randint() function from the random module. For example, random.randint(1, 6) would generate a random integer between 1 and 6, simulating the roll of a single die. To calculate the probability of rolling a specific number over a large number of trials, you can use the formula: probability = (number of times the event occurs) / (total number of trials). You can use a loop to simulate multiple dice rolls and calculate the probability of rolling a specific number.

import random

# Simulate rolling a single die
roll = random.randint(1, 6)
print("You rolled a", roll)

# Simulate rolling multiple dice and calculate the probability of rolling a specific number

num_trials = 1000
num_successes = 0
for i in range(num_trials):
    roll = random.randint(1, 6)
    if roll == 6:
        num_successes += 1

probability = num_successes / num_trials
print("The probability of rolling a 6 is", probability)
