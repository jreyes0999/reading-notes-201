# Control flow
* The control flow is the order in which the computer executes statements in a script.
* A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.
* Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.
* For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:
```
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
```
## Operators
* JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.
- Assignment operators
- Comparison operators
- Arithmetic operators
- Bitwise operators
- Logical operators
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators
* JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. A binary operator requires two operands, one before the operator and one after the operator:
```
operand1 operator operand2
3+4 or x*y
```
* A unary operator requires a single operand, either before or after the operator.
    * operator operand (x++)
    * operand operator (++x)
## Comparison operators
* Equal (==)	Returns true if the operands are equal.
* Not equal (!=)	Returns true if the operands are not equal.
* Strict equal (===)	Returns true if the operands are equal and of the same type
* Strict not equal (!==)	Returns true if the operands are of the same type but not equal, or are of different type.
## Arithmetic operators
* An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value
    * Remainder (%)	- Binary operator. Returns the integer remainder of dividing the two operands.
    * Increment (++) - Unary operator. Adds one to its operand. If used as a prefix operator (++x), returns the value of its operand after adding one; if used as a postfix operator (x++), returns the value of its operand before adding one.
    * Decrement (--) - Unary operator. Subtracts one from its operand. The return value is analogous to that for the increment operator.
    * Unary negation (-) - Unary operator. Returns the negation of its operand.
    * Unary plus (+) - Unary operator. Attempts to convert the operand to a number, if it is not already.
    * Exponentiation operator (**) - Calculates the base to the exponent power, that is, base^exponent
## Logial Operators
* Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value.\
    * Logical AND (&&) - expr1 && expr2	Returns expr1 if it can be converted to false; otherwise, returns expr2. Thus, when used with Boolean values, && returns true if both operands are true; otherwise, returns false.
    * Logical OR (||) - expr1 || expr2	Returns expr1 if it can be converted to true; otherwise, returns expr2. Thus, when used with Boolean values, || returns true if either operand is true; if both are false, returns false.
    * Logical NOT (!) - !expr	Returns false if its single operand that can be converted to true; otherwise, returns true.
**&& Operator**
```
var a1 =  true && true;     // t && t returns true
var a2 =  true && false;    // t && f returns false
var a3 = false && true;     // f && t returns false
var a4 = false && (3 == 4); // f && f returns false
var a5 = 'Cat' && 'Dog';    // t && t returns Dog
var a6 = false && 'Cat';    // f && t returns false
var a7 = 'Cat' && false;    // t && f returns false
```
**|| Operator**
```
var o1 =  true || true;     // t || t returns true
var o2 = false || true;     // f || t returns true
var o3 =  true || false;    // t || f returns true
var o4 = false || (3 == 4); // f || f returns false
var o5 = 'Cat' || 'Dog';    // t || t returns Cat
var o6 = false || 'Cat';    // f || t returns Cat
var o7 = 'Cat' || false;    // t || f returns Cat
```
**! Operator**
```
var n1 = !true;  // !t returns false
var n2 = !false; // !f returns true
var n3 = !'Cat'; // !t returns false
```

## String operators
* In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.
```
console.log('my ' + 'string'); // console logs the string "my string".
```

## Functions
* Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.
* A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:
    * The name of the function.
    * A list of parameters to the function, enclosed in parentheses and separated by commas.
    * The JavaScript statements that define the function, enclosed in curly brackets, {...}.
```
function square(number) {
  return number * number;
}
```
* Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:
```
square(5);
```
* Functions must be in scope when they are called, but the function declaration can be hoisted (appear below the call in the code), as in this example:
```
console.log(square(5));
/* ... */
function square(n) { return n * n }
```