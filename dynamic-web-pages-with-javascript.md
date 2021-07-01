# JavaScript Notes
   * JavaScript (JS) is a lightweight, interpreted, or just-in-time compiled programming language with first-class functions.
   * While it is most well-known as the scripting language for Web pages, many non-browser environments also use it, such as Node.js, Apache CouchDB and Adobe Acrobat
   * JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.
    * The standards for JavaScript are the ECMAScript Language Specification (ECMA-262) and the ECMAScript Internationalization API specification (ECMA-402).

## Prompting the User Notes
   * The function prompt accepts two arguments: 
```
result = prompt(title, [default]);
```
   * Summary
      - alert: shows a message
      - prompt: shows a message asking the user to input text. It returns the text or, if Cancel button or Esc is clicked, null.
      - confirm: shows a message and waits for the user to press “OK” or “Cancel”. It returns true for OK and false for Cancel/Esc.
    * All these methods are modal: they pause script execution and don’t allow the visitor to interact with the rest of the page until the window has been dismissed.

## Boolean conversion
   * The so-called “conditional” or “question mark” operator lets us do that in a shorter and simpler way.
   * The if(...) statement evaluates a condition in parentheses and, if the result is true, executes a block of code.
```
let year = prompt('In which year was ECMAScript-2015 specification published?', '');

if (year == 2015) alert( 'You are right!' );
```
   * If we want to execute more than one statement, we have to wrap our code block inside curly braces:
```
if (year == 2015) {
  alert( "That's correct!" );
  alert( "You're so smart!" );
}
```
   * The operator is represented by a question mark ?. Sometimes it’s called “ternary”, because the operator has three operands. It is actually the one and only operator in JavaScript which has that many.
   * A number 0, an empty string "", null, undefined, and NaN all become false. Because of that they are called “falsy” values. Other values become true, so they are called “truthy”.
   * So, the code under this condition would never execute:
```
if (0) { // 0 is falsy
  ...
}
```
   * And inside this condition it always will. 
```
if (1) { // 1 is truthy
  ...
}
```
   * The "else" clause: The if statement may contain an optional “else” block. It executes when the condition is falsy.
```
let year = prompt('In which year was the ECMAScript-2015 specification published?', '');

if (year == 2015) {
  alert( 'You guessed it right!' );
} else {
  alert( 'How can you be so wrong?' ); // any value except 2015
}
```
   * Sometimes, we’d like to test several variants of a condition. The else if clause lets us do that.
```
let year = prompt('In which year was the ECMAScript-2015 specification published?', '');

if (year < 2015) {
  alert( 'Too early...' );
} else if (year > 2015) {
  alert( 'Too late' );
} else {
  alert( 'Exactly!' );
}
```
   * In the code above, JavaScript first checks year < 2015. If that is falsy, it goes to the next condition year > 2015. If that is also falsy, it shows the last alert. There can be more else if blocks. The final else is optional.
   * 
## Conditional operator ‘?’
   * Sometimes, we need to assign a variable depending on a condition.
```
let accessAllowed;
let age = prompt('How old are you?', '');

if (age > 18) {
  accessAllowed = true;
} else {
  accessAllowed = false;
}

alert(accessAllowed);
```
   * The syntax is as follows:
``` 
let result = condition ? value1 : value2;
```
   * The condition is evaluated: if it’s truthy then value1 is returned, otherwise – value2.
```
let accessAllowed = (age > 18) ? true : false;
```
   * A sequence of question mark operators ? can return a value that depends on more than one condition.
```
let age = prompt('age?', 18);

let message = (age < 3) ? 'Hi, baby!' :
  (age < 18) ? 'Hello!' :
  (age < 100) ? 'Greetings!' :
  'What an unusual age!';

alert( message );
```
![Example](https://flux.s-ul.eu/Qct1EhU4.png)

## JavaScript Variables
   * There are 3 ways to declare a JavaScript variable:
      * Using var
      * Using let
      * Using const
   * Variables are containers for storing data (values).
```
var x = 5;
var y = 6;
var z = x + y;
```
## JavaScript identifiers
   * All JavaScript variables must be identified with unique names. These unique names are called identifiers.
   * The general rules for constructing names for variables (unique identifiers) are:
      * Names can contain letters, digits, underscores, and dollar signs.
      * Names must begin with a letter
      * Names can also begin with $ and _ (but we will not use it in this tutorial)
      * Names are case sensitive (y and Y are different variables)
      * Reserved words (like JavaScript keywords) cannot be used as names
   * The equal sign (=) is an "assignment" operator, not an "equal to" operator. 
   * Since JavaScript treats underscore as a letter, identifiers containing _ are valid variable names:
``` 
var _lastName = "Johnson";
var _x = 2;
var _100 = 5;
```