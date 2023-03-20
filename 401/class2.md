# README.md

## Read Assignment 2

In Tests We Trust — TDD with Python
Gomes (2017) stated that unit tests are "some pieces of code to exercise the input, the output and the behavior of your code", it can be written at any time. However, the strategy to think and write is called the Test-Driven Development. TDD is a development of tests (testing a feature); it is advisable to run tests before adding that feature to your code.

For example, if you developed an API connection that identifies possible genders, the code needs to return the possible gender as the output (once the name is entered). Therefore, writing a test is important, meaning writing a code/function to test it. The test name must state "what is expected and what we are testing" (Gomes, 2017).

The author, Gomes, also mentioned in her article that the test file should "follow the same name of module name", so if the module is named first_module.py, then the test name should be test_first_module.py.

module/
- first_module.py

tests/
- test_first_module.py

Another important thing to consider is the structure, and one of the widely used is the AAA (Arrange, Act, and Assert). Gomes (2017) describes AAA as follows:

Arrange - organizing the data needed to execute the input, for example, or any piece of code
Act - executes the code that is being tested
Assert - once the code is executed, always check if the output or result meets what is expected
Once all these three are ready, the tests can be executed using pytest (or any other).

The Cycle
The cycle's three steps (Gomes, 2017):

write a unit test; it should fail because the feature is not there yet
write the feature; this will make the test pass
refactor the code
This cycle can be repeated every time a feature is added or modified.
What does the if name == “main”: do?
The __name == "main" will execute the code when the file runs as a script and not when imported as a module. The python interpreter reads the source file before executing the code and defines special or global variables before executing (Shah, (n.d.)). If that module or source file is what the python interpreter runs as the main program, then "it sets the special name variable to have a value “main” " (Shah, (n.d.)).

However, if the file is imported from a different or another module, then the name will be set to that module's name (Shah, (n.d.)). In her article, Shah (n.d.) describes

Introduction to Recursion – Data Structure and Algorithm Tutorials
A function that calls itself is called recursion, while the "corresponding function is called a recursive function" (Geeks for Geeks, 2022). It reduces the length of the code, making it easier.

## Things I want to know more about 

 Recursion
