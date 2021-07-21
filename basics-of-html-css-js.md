# Basics of HTML, CSS, and JavaScript

## HTML
- When creating a web page you add tags to the contents of the page
- Tags allow for your webpage to be "assembled" a certain way, based on what tags are used. 
- Structural Markup: Elements that are used to describe headins and paragraphs.
- Semantic Markup: Introduces meaning to the web page rather than just presentation.

## HTML Tag List
- Headings vary from sizes 1-6 
- Headings are created with an opening and closing tag. `(<h1></h2>)`
- Paragraph tag `(<p></p>)`
- Bold tag `(<b></b>)`
- Italic tag  `(<i></i>)`

## CSS
- CSS is used to style your webpage.
- A CSS rule contains two parts: a **selector** and a **declaration**
- Selectors are HTML elements you want to style (h1, h2, or p)
- Declaration tells the webpage how is should be styled. 
- CSS declarations contain **property** and **value**, separated by a colon

`h1 {
    font-family: Arial;
    color: yellow;
}`

- Properties are pretty much basic things like the color of the text, the font, the width, the height, and the border. 
- Values are what exactly is being changed about the selector, such as making the h1's yellow.

## List of CSS Selectors

- `* {}`: This targets all elements on a page.
- `h1. h2, h3 {}`: This targets specific elements on a page.
- `.note {}`: This targets all elements whose class has the *note* value.
- `#introduction {}`: This targets the element with the id value of *introduction*. 
-  Basically `*` can be used to style all elements on your page, and `.` or `#` are used to style specific elements!

## JavaScript
### Basic JavaScript Instructions
- A *script* is a set of step by step instructions written for the computer to follow.
- A script temporarily stores info in **variables**.
- Use *let* to declare a variable that may change.
- Use *const* to declare a variable that will remain the same.
- A variable's name should describe the kind of data the variable holds.
 
`let quantity = 3;`

## JavaScrpt Data Types
- Number: includes all numbers, positive, negative, and decimals
- String: anything inside quotation marks 'What is you name?'
- Boolean: only have a true or false value

**How to use a variable to store a number**

`var price;`
`var quantity;`
`var total;`

`price = 5;`
`quantity = 14;`
`total = price * quantity;`

`var el = document.getElementById('cost');`
`el.textContent = '$' + total;`

## Boolean Info
- A Boolean variable can only be True or False.
- Booleans are only used when something can only be T/F.

## Variable Name Rules
- The name must begin with a letter, `$` or an `_`.
- It cannot start with a number.
- You cannot use a dash, periods, or keywords. 
- You cannot use keywords or reserved words.

## Arrays
- An *array* stores a list of  values.
- Arrays are used whenever you are working with a set of list of values that are related.
- Values in an array are separated by commas.

`var colors;`
`colors = ['white', 'black', 'custom'];`

`var el = document.getElementById('colors');`
`el.textContent = colors[0];`

- Give the array a name.
- Values are assigned to the array inside a pair of brackets [*values go here*]
- A boolean, number, and string can go in the same array because values in an array do not have to be the same data type.
- Each array has a property called **length**, which holds the number of items in the array.
- You can change the value of an item in an array by selecting it and assigning it a new value.

## Expressions
- An expression evaluates into a single value.

`var area = 3 * 2;`

## List of Operators
- Expressions rely on **operators** 
- Assignment Operators: `=`
- Arithmetic Operators: `*`
- String Operators: `greeting = 'Hi ' + 'Molly';`
- Comparison Operators: `buy = 3 > 5;`
- Logical Operators: `buy = (5 > 3) && (2 < 4);`

## Decisions & Loops
- In a script the code can take more than one path
- To determine which path to take, programs often rely upon the following three concepts
- **Evaluations:** Analyze if values match expected results
- **Decisions:** Use the results of evaluations to decide which path the script should go
- **Loops:** Perform the same steps repeatedly

## Conditional Statements

- Conditional Statements are based on the if/then/else concept
- If a condition is met, then your code executes one or more statements, else your code does something different or just skips the script

## Comparison Operators

- `===` Strict Equal to  
- `!==` Strict NOT equal to

## Logical Operators

- `&&` Logical AND tests if two expressions evaluate to true. If one expression is false, then the whole thing returns false!
- `||` Logical OR tests if one of two expressions evaluates to true. If at least one IS true, the entire expression returns true





