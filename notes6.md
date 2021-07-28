# HTML Tables; JS Constructor Functions

- What is domain modeling?
Domain modeling is the process of creating a conceptual model in code for a specific problem. And a domain problem that's articulated well can verify your understanding of that problem.

- What is an Object-Oriented model?
An entity that stores data in properties and behaviors in methods.

- How to learn to implement domain models in JavaScript?
Write out and test your code so that you can remember how to implement doamin models in JS.

- How to define the same properties between many objects?
Use a constructor function.

**Storing data within properties makes it possible for any new object to access that data later.**

## What is object-oriented programming in JavaScript?
1. creating an object
2. initializing properties inside object using the `this` variable
3. store the object in a variable for later use

- What can a random number generator be used for?
A random number generator can be used to model the random nature of user behavior.

- What function can be used to generate a random number?
`Math.random()`

- Why use a prototype and what is it?
A prototype is like an object's stunt double, you can use it to store methods. It is considered best practice in JavaScript to locate a method on the prototype object. In addition to that it allows two objects to share the same code, which makes a running program consume less memory. Consuming less memory is important for devices like smart phones and tablets.

- Tips to follow when building domain models
1. Build self containted objects with the same properties and methods.
2. Model its properties with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the `new` keyword followed by a call to a constructor function.
5. Store the new object in a variable so that you can access its properties and methods from outside.
6. Use the `this` variable in your methods so you can access the object's properties and methods from inside.


- How to create an object using constructor notation:
 `let car = new Object();`
 `car.name = 'Toyota';`
 `car.model = 'Prius';`
 `car.mileage = 400;`
 `car.milesPerGallon = 50;`
 `car.checkGasNeeded = function() {`
     `this.mileage/this.milesPerGallon;`
 `}`

 **To create an empty object using literal notation use:**
 `let car = {} (curly braces)`
*The curly braces create an empty object*

- How to update an object?
  - use dot notation or square brackets like this: hotel.name = 'Park';
  - dot notation & square brackets work on objects created using literal or constructor notation
  - to delete a property use the *delete* keyword like this: `delete hotel.name;`
  - to clear the value of a property do this: `hotel.name = '';`

- How to create many objects
Many objects can be created by using *Object Construtctor Notation*

- What is `this`?
It is a keyword used inside of functions and objects. It always refers to one object!

- When is a function global?
A function has a global scope when it is created at the top level of a script(not inside another object or function).

- When does a function become a method?
When a function is defined inside of an object it becomes a method.

- How is data represnted in JavaScript?
In JavaScript data is represented using name/value pairs.

- How can you organize your data in JavaScript?
To organize your data, you can use an array or object to group a set of related values.

- What is a name also known as in arrays and objects?
In arrays and objects the name is also known as a key.







