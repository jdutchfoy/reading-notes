# README.md

## Read Assignment 3

### Readings: FileIO & Exceptions

Reading and Writing Files in Python (Guide)
One of the common tasks in coding is reading and writing files. According to Mertz (n.d.), "a file is a contiguous set of bytes used to store data"; this file can be a text file or an executable program.
Three main parts of modern file system (Mertz, n.d.):
Header
Data
EOF or End of file
The header is a metadata about file contents, the data contains file or information written by the creator, while end of file is a " special character that indicates the end of the file" (Mertz, n.d.).
File Path
The file path is required to access the file:
Folder path - folder's location in the system/device
File name - the name of the file
Extension - "the end of the file path pre-pended with a period (.) used to indicate the file type" (Mertz, n.d.).

Create a File

open("sample.text") or
file = open("sample.text")

Close

reader = open('dog_breeds.txt')
try: # Further file processing goes here
finally:
reader.close()

Exceptions in Python

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.
Exceptions versus Syntax Errors
Syntax errors occur when the parser detects an incorrect statement. The arrow indicates where the parser ran into the syntax error.
Exception Error: This type of error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into. Instead of showing the message exception error, Python details what type of exception error was encountered. Python comes with various built-in exceptions as well as the possibility to create self-defined exceptions.
Raising an Exception
We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception. The program comes to a halt and displays our exception to screen, offering clues about what went wrong.
The AssertionError Exception
Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met.
The try and except Block: Handling Exceptions
The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause. When syntactically correct code runs into an error, Python will throw an exception error. This exception error will crash the program if it is unhandled. The except clause determines how your program responds to exceptions.
The else Clause
In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.
Cleaning Up After Using finally
Everything in the (finally) clause will be executed. It does not matter if you encounter an exception somewhere in the try or else clauses.

## Things I want to know more about
