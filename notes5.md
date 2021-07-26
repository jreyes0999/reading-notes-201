# Problem Domain, Objects, and the DOM

## What is inside of an object?
- Inside of an object variables become properties, and functions become methods.
- Objects contain a set of variables and functions that create a model of something in the real world.

## How do you create an object?

- You define and create a JavaScript object with an object literal:
`const person = {firstName:"John" , lastName:"Doe", age:50, eyeColor:"blue"};`

- Space and line breaks don't matter!! An object can be on multiple lines in your code editor like this:

`const person = {`
    `firstName: "John",`
    `lastName: "Doe",`
    `age: 50,`
    `eyeColor: "blue"`
`};`

- Separate each key from its value using a colon
- Separate each property and method with a comma (but not after the last value)

## What are some object rules?
- An object cannot have two keys with the same name, because keys are used to access their corresponding values.
- The value of a property can be a string, number, Boolean, array, or even another object
- The value of a method is always a function

## What is the object?
- Objects are the curly braces and their contents
- Objects are stored in a variable

*this*: is a keyword.

## How to access an object?
- Use dot notation:

`var mallName = mall.name;` (In this example mall is the object & *name* is the property)

`var mallName = mall.checkStoreHours();` (In this example mall is the object & checkStoreHours(); is the method aka function)

- You can also use square brackets:

`var hotelName = hotel['name'];`
`var roomsFree = hotel['checkAvailability']();`

- Square brackets are only used to access an object if: name or method contains special characters, the name is a number, or if a variable is being used instead of a property name

- If you have more than one object modeling the same thing the same code can be used just do the property changes needed, and make sure you change the name of the object!

## Why would someone use an object?
- To create a model of something in the real word such as a shirt, a car, a hotel, and the list does on!

# Problem Domain
- Understanding the problem is the **MOST** critical piece to coding. 
- Make sure to understand the problem inside and out **BEFORE** trying to solve it with code. 

# Document Object Model

## What does the Document Object Model do?
- It specifies how the browser should create a model of the HTML page, and how JavaScript can access and update the contents of a web page while in a browser window.
- The DOM specifies the way a browser should structure the HTML model using a DOM tree.

## What is the DOM?
- It's not a part of HTML or JavaScript
- It's a separate set of rules

## Why is the DOM called an object model?
- Because it's made of objects (each object represents a different part of the page loaded in the browser window)

## What is the DOM also known as?
- An *Application Programming Interface* (API)

## What do API's do?
- API's let programs and scripts talk to each other
(Example: The DOM states what your script can ask the browser about the current page. and how to tell the browser to update what is being shown to the user)

## What is the DOM tree?
- The DOM represents HTML as a tree structure of tags. Here’s how it looks:
```
<!DOCTYPE HTML>
<html>
<head>
  <title>About elk</title>
</head>
<body>
  The truth about elk.
</body>
</html>
```

HTML
HEAD
#text ↵␣
TITLE
#text About elk
#text ↵
#text ↵
BODY
#text The truth about elk.
