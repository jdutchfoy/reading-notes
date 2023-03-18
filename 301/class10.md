# README.md

## Read Assignment 10

1.The call stack is used every time a function is invoked, each done "one at a time, from top to bottom ". The call stack is synchronous.

2.The function execution is only done one at a time.

3.LIFO stands for Last In, First Out, a data structure that the call stack uses to store and manage function calls temporarily .

4.function sayHi(name) { console.log(Greetings to you ${name}!); }

const greetings1 = sayHi('Ella');

sayHi

global

callstack

5.The function sayHi() doesn’t cross the stack until it is called/invoked in line 24. Lines 20-22 are only a function declaration - function sayHi(name){...}. Line 24 is where you declare a variable greetings1 and assign it to the evaluated result of invoking the function sayHi() passing in the arguments 'Ella'.

6.A reference error is when you use a variable that is not defined or declared.

1.Syntax errors cannot be parsed; a good example would be missing a semi-colon or having trailing commas or spaces .

2.Range errors exist when manipulating data or objects, giving "it an invalid length"

3.Type errors occur when "the types (number, string, and so on) you are trying to use or access are incompatible"

4. A breakpoint is achieved by placing "a debugger statement in your code in the line you want to break 2Links to an external site.".
