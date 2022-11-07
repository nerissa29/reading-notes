## Reading Notes 09

## Functional Programming Concepts

### What is functional programming?

It is "a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data" - [Wikipedia: Functional programming](https://en.wikipedia.org/wiki/Functional_programming) and [Medium: Concepts of Functional Programming in Javascrip](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa).

### What is a pure function, and how do we know if something is a pure function?

It is a pure function when [^2]:

- if given the same arguments, it returns the same results
- there are no observable side effects

The pure function also is referred to as *deterministic* [^2].

### What are the benefits of a pure function?

The benefits of Pure Function according to [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa):

- it is easier to test
- no need to mock anything, and
- unit test pure functions with:
  - "Given a parameter A → expect the function to return value B [^2]"
  - "Given a parameter C → expect the function to return value D [^2]"

### What is immutability?

Immutability means the data cannot change after it's created [^2]. When data is immutable, you cannot change it. However, one can create a new object with a new value [^2]. 

### What is Referential transparency?

*'pure functions + immutable data = referential transparency'* - [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

If an expression is referentially transparent, it can be replaced with its value - or vice, modifying the program/system's behavior.

## Node JS Tutorial for Beginners #6 - Modules and require()

### What is a module?

A module is a file containing related codes.

#### What does the word ‘require’ do?

The *require()* is a NodeJS built-in statement that reads and executes the JavaScript file/modules and returns the exported object.

#### How do we bring another module into the file we are working in?

We first need to export the component from its file (file A), then import it to another file (file B) as *import Book from './file-path.name'*. We then now can use the imported component into our file B.

#### What do we have to do to make a module available?'

Inside the module, we need to do a *module.export = "part of the module you want to export*. The next step will be requiring it on the file (external file) that needs access to that module:

*ex. cost name = require('./module’s path');


[^1]: [Wikipedia: Functional programming](https://en.wikipedia.org/wiki/Functional_programming)
[^2]: [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

