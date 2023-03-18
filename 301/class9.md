# README.md

## Jan 22 at 4:36pm

Read Assignment 9

1.It is "a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data"

2.It is a pure function when 1Links to an external site.:

if given the same arguments, it returns the same results
there are no observable side effects
The pure function also is referred to as deterministic

3.The benefits of Pure Function

         it is easier to test

no need to mock anything, and
unit test pure functions with:
"Given a parameter A → expect the function to return value B 1Links to an external site."
"Given a parameter C → expect the function to return value D 1Links to an external site."
4.Immutability means the data cannot change after it's created. When data is immutable, you cannot change it. However, one can create a new object with a new value.

5.'pure functions + immutable data = referential transparency'

If an expression is referentially transparent, it can be replaced with its value - or vice, modifying the program/system's behavior.

1.A module is a file containing related codes.

2.We first need to export the component from its file (file A), then import it to another file (file B) as import Book from './file-path.name'. We then now can use the imported component into our file B.

3.Inside the module, we need to do a module.export = "part of the module you want to export. The next step will be requiring it on the file (external file) that needs access to that module:
