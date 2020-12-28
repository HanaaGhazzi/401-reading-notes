# Classes, Inheritance, Functional P..

#### Can JavaScript be used outside of a browser?
_Node. js is a free, open-source JavaScript runtime. ... Well, it means that it allows JavaScript to run outside of the browser and in any platform. Any JavaScript code that one writes will run in any system that has Node_

#### What is the difference between a module and a package?

_A module is a single file (or files) that are imported under one import and used. ... A package is a collection of modules in directories that give a package hierarchy._

#### What does the node package manager do?
_Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node._

#### Export Function:


**You can attach an anonymous function to exports object as shown below.**
``` 
module.exports = function (msg) { 
    console.log(msg);
};

```
**Now, you can use the above module, as shown below.**
```
var msg = require('./Log.js');

msg('Hello World');
```
**Export Function as a Class**
```
module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}
```

### Vocabulary Terms:


|  Terms   	|     Defination   	|
|---	|---	|
|   Ecosystem:	|   A collection of software projects, which are developed and co-evolve in the same environment. The environment can be organizational (a company), social (an open-source community), or technical (like NPM).	|
|   Node.js:	|    An asynchronous event-driven javaScript runtime.   |
|   V8 Engine:	|  JavaScript environment used in Google Chrome 	|
|   Module:	|   A module is any file or directory in the node_modules directory that can be loaded byt the Node.js require() function	|
|   Package: 	|    A package is a file or directory that is described by a package.json file. A package must contain a package.json file.	|
|  Node Package Manager (NPM): 	|    A command line tool that installs, updates, or uninstalls Node.js packages in applications. It's also an online repository for open-source Node.js projects.|
|   Server:	|   a computer or computer program which manages access to a centralized resource or service in a network.	|
|   Environment:	|   A combination of software and hardware in a computer.|
|   Interpreter:	|  A program that directly executes instruction written in a programming or scripting language, without requiring them previously to have been compiled into a machine language program. |
|   Compiler:	|    A program that translates computer code written in one programming language (the source language) into another language (the target language).	|

