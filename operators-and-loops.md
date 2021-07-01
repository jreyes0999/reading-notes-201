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
## Assignment operators
* An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.
    * Assignment `x = y	 x = y`
    * Addition assignment `x += y	x = x + y`
    * Subtraction assignment `x -= y  x = x - y`
    * Multiplication assignment	`x *= y	 x = x * y`
    * Division assignment `x /= y  x = x / y`
    * Remainder assignment `x %= y  x = x % y`
## Comparison operators
* Equal (==) - Returns true if the operands are equal.
* Not equal (!=) - Returns true if the operands are not equal.
* Strict equal (===) - Returns true if the operands are equal and of the same type
* Strict not equal (!==) - Returns true if the operands are of the same type but not equal, or are of different type.
* Greater than (>) - Returns true if the left operand is greater than the right operand.
* Greater than or equal (>=) - Returns true if the left operand is greater than or equal to the right operand.
* Less than (<)	- Returns true if the left operand is less than the right operand.
Less than or equal (<=)	- Returns true if the left operand is less than or equal to the right operand.
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
* The shorthand assignment operator += can also be used to concatenate strings.
```
var mystring = 'alpha';
mystring += 'bet'; // evaluates to "alphabet" and assigns this value to mystring.
```