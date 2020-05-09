## Everything is an object
- In javascript we have two types of values
    - primitives : Numbers, String, undefined, null, Boolean
    - objects : Arrays, Functions, Objects, Dates, Wrappers for Numbers/Strings
    
## Object-Oriented Programming
   - Object interacts with each other through method properties
   - Used to store data, structure applications into module and keeping code clean

## Inheritance 
 - Javascript is a prototype based language which means inheritance is used by using prototypes
 - Each javascript object has prototype property which makes inheritance possible in javascript.
 - The prototype property of an object is where we put  methods and properties that we want other objects to inherit.
 - Each object in javascript is a instance of Object constructor(object) just like java

### Prototype Chaining
 - It is inheritance, object is linked to each other. Inheritance work in java from bottom to top. If method is not present in current object then it looks in then its prototype(super class).If it does find the method even in object object then it will go to null. Null is final link in the prototype chain.
 
#### Function Constructor
 - The Function constructor creates a new Function object. Calling the constructor directly can create functions dynamically, but suffers from security and similar (but far less significant) performance issues to eval. However, unlike eval, the Function constructor creates functions which execute in the global scope only.
 - Sometimes we need a "blueprint" for creating many objects of the same "type". The way to create an "object type", is to use an object constructor function.

### Object.create()
    The Object.create() method creates a new object, using an existing object as the prototype of the newly created object.

### Object.create() vs function constructor
    The difference is Object.create builds an object that inherits that we directly passed into the first argument while on the other hand the functional constructor, the newely created objects inherit from the constructor prototype property. 

### Function
   - A function is an instance of the Object type.
   - A function behaves like any other object.
   - We can store functions in a  variable.
   - We can pass a function as an argument to another function.
   - We can return a function from function.
   
### Closure
    - An inner function has always access to the variables and parameters of its outer function, even  after  the outer function has returned.

### call() apply() bind()

- Call method is used to call a function of different method. It takes 'this' as an argument.
- Apply method serves the same purpose, instead it takes an arrays argument.
- Bind method also serves the same purpose, but unlike call method it does not immediatly call the function instead it generates the copy of object, so that it can store preset.
