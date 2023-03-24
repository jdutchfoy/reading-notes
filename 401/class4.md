## README.md

### Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

## Accessing Object Variables

You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class.

## Accessing Object Functions

To access a function inside of an object you use notation similar to accessing a variable.

init()

The init() function, is a special function that is called when the class is being initiated. It's used for asigning values in a class.

Thinking Recursively
Recursive Functions in Python

A recursive function is a function defined in terms of itself via self-referential expressions. This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case. Behind the scenes, each recursive call adds a stack frame (containing its execution context) to the call stack until we reach the base case. Then, the stack begins to unwind as each call returns its results.

## Maintaining State

When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

Thread the state through each recursive call so that the current state is part of the current call’s execution context
Keep the state in global scope
Recursive Data Structures in Python

A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure. Using the empty list and the attach_head operation, you can generate any list. List is not the only recursive data structure. Other examples include set, tree, dictionary, etc.

Recursive data structures and recursive functions go together like bread and butter. The recursive function’s structure can often be modeled after the definition of the recursive data structure it takes as an input.

Naive Recursion is Naive

The Fibonacci numbers were originally deﬁned by the Italian mathematician Fibonacci in the thirteenth century to model the growth of rabbit populations. Fibonacci surmised that the number of pairs of rabbits born in a given year is equal to the number of pairs of rabbits born in each of the two previous years, starting from one pair of rabbits in the ﬁrst year. Naively following the recursive deﬁnition of the nth Fibonacci number was rather inefficient. As you can see from the output above, we are unnecessarily recomputing values. lru_cache is a decorator that caches the results. Thus, we avoid recomputation by explicitly checking for the value before trying to compute it. One thing to keep in mind about lru_cache is that since it uses a dictionary to cache results, the positional and keyword arguments (which serve as keys in that dictionary) to the function must be hashable.

### Pesky Details

Python doesn’t have support for tail-call elimination. As a result, you can cause a stack overflow if you end up using more stack frames than the default call stack depth. Keep this limitation in mind if you have a program that requires deep recursion. Also, Python’s mutable data structures don’t support structural sharing, so treating them like immutable data structures is going to negatively affect your space and GC (garbage collection) efficiency because you are going to end up unnecessarily copying a lot of mutable objects.

