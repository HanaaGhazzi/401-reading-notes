# Data Modeling & NoSQL Database .. 

#### Name 3 advantages to Test Driven Development : 
- Improved Focus

- Better code quality

- Flexible and modular code

#### In what case would you need to use beforeEach() or afterEach() in a test suite?

in the case of repeating Setup For Many Tests: If you have some work you need to do repeatedly for many tests, you can use beforeEach and afterEach.

#### What is one downside of Test Driven Development

- Big time investment. For the simple case you lose about 20% of the actual implementation, but for complicated cases you lose much more.

- Additional Complexity. For complex cases your test cases are harder to calculate, I'd suggest in cases like that to try and use automatic reference code that will run in parallel in the debug version / test run, instead of the unit test of simplest cases.

#### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

The difference between classical inheritance and prototypal inheritance is that classical inheritance is limited to classes inheriting from other classes, while prototypal inheritance supports the cloning of any object using an object linking mechanism.

#### Name a use case for a static method

The best use case for static methods in other languages is to group functions (that aren't really object-oriented and don't work on objects) together into classes for convenience and to create "alternate" constructors that are associated with the class their intended to construct.

#### Write an example of a Higher Order function and describe the use case it solves

The map function is one of the many higher-order functions built into the language. sort, reduce, filter, forEach are other examples of higher-order functions built into the language. 

```
[1, 2, 3, 4].map(function(n){
    return n * 2
})
```

### Vocabulary Terms:

|  Terms   	|     Defination   	|
|---	|---	|
|   functional programming:	|   Ais the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions.	|
|   pure function:	|    is a function which Given the same inputs, always returns the same output, and Has no side-effects   |
|  higher order function:	|  is any function which takes a function as an argument, returns a function, or both.	|
|  immutable state:	|  Immutable data cannot change its structure or the data in it.	|
|   Objects: 	|    are complex and each object may contain any combination of the primitive data-types as well as reference data-types.and objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, in the form of “key: value” pairs.|
|  Object-oriented programming (OOP): |    is a programming paradigm based on the concept of "objects", In OOP, computer programs are designed by making them out of objects that interact with one another.|
|   class:	|   is an extensible program-code-template for creating objects	|
|   prototype:	|    is a property can be used to add methods to existing constructors.|
|   ``super:``	|  a keyword used to access and call functions on an object's parent. When used in a constructor, the super keyword appears alone and must be used before the this keyword is used. |
|   inheritance: 	|   is the mechanism of basing an object or class upon another object.	|
|   constructor: 	|   In class-based object-oriented programming, a constructor is a special type of subroutine called to create an object|
|   instance:	|    In object-oriented programming (OOP), an instance is a concrete occurrence of any object, existing usually during the runtime of a computer program.|
|   context:	|  Context is always the value of the this keyword which is a reference to the object that “owns” the currently executing code or the function where it’s looked at. |
|   ``this:``	|    A property of an execution context (global, function or eval) that, in non–strict mode, is always a reference to an object and in strict mode can be any value.	|
|   Test Driven Development (TDD):	|    is a software development process that relies on the repetition of a very short development cycle: requirements are turned into very specific test cases, so its an evolutionary approach to development which combines test-first development .|
|   Jest:	| is a JavaScript Testing Framework |
|   Continuous Integration (CI):	|     is a development practice where developers integrate code into a shared repository frequently, preferably several times a day	|
|  unit test:	|   is a level of software testing where individual units/ components of a software are tested.The purpose is to validate that each unit of the software performs as designed.	|


