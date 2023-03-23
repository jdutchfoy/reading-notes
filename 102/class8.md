## Operators and Loops

At a high level, an expression is a valid unit of code that resolves to a value. There are two types of expressions: those that have side effects (such as assigning values) and those that purely evaluate.

The expression x = 7 is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. The expression itself evaluates to 7.

The expression 3 + 4 is an example of the second type. This expression uses the + operator to add 3 and 4 together and produces a value, 7. However, if it's not eventually part of a bigger construct (for example, a variable declaration like const z = 3 + 4), its result will be immediately discarded — this is usually a programmer mistake because the evaluation doesn't produce any effects.

As the examples above also illustrate, all complex expressions are joined by operators, such as = and +. In this section, we will introduce the following operators:

The precedence of operators determines the order they are applied when evaluating an expression. For example:

const x = 1 + 2 *3;
const y = 2* 3 + 1;

The precedence of operators determines the order they are applied when evaluating an expression. For example:

Assignment operators
An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

There are also compound assignment operators that are shorthand for the operations listed in the following table:

Name Shorthand operator Meaning
Assignment x = f() x = f()
Addition assignment x += f() x = x + f()
Subtraction assignment x -= f() x = x - f()
Multiplication assignment x *= f() x = x* f()
Division assignment x /= f() x = x / f()
Remainder assignment x %= f() x = x % f()
Exponentiation assignment x **= f() x = x** f()
Left shift assignment x <<= f() x = x << f()
Right shift assignment x >>= f() x = x >> f()
Unsigned right shift assignment x >>>= f() x = x >>> f()
Bitwise AND assignment x &= f() x = x & f()
Bitwise XOR assignment x ^= f() x = x ^ f()
Bitwise OR assignment x |= f() x = x | f()
Logical AND assignment x &&= f() x && (x = f())
Logical OR assignment x ||= f() x || (x = f())
Nullish coalescing assignment x ??= f() x ?? (x = f())
Assigning to properties
If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. For example:

const obj = {};

obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }.

If an expression does not evaluate to an object, then assignments to properties of that expression do not assign:

const val = 0;
val.x = 3;

console.log(val.x); // Prints undefined.
console.log(val); // Prints 0.

## Things I want to know more of


