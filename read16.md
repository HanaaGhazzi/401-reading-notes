# Event Driven Applications

## Event-Driven Programming in Node.js

**Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.**

 #### Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be called when an event is triggered.

- A Main Loop listens for event triggers and calls the associated event handler for that event.

![event](https://thecodersblog.com/uploads/687474703a2f2f692e737461636b2e696d6775722e636f6d2f4c6273397a2e706e6770.png)

Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter. We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

- EventEmitter that allows us to get started incorporating Event-Driven  Programming in our project right away.
- In node.js an event can be described as a string with a corresponding callback.
- An event can be “emitted” multiple times we can choose to only listen for the first time event is emitted.

```const EventEmitter = require('events').EventEmitter```
``` const myEventEmitter = new EventEmitter```

### Object Oriented Programming + Event-Driven Programming

These two make for a very valuable combination in a wide variety of situations. The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

