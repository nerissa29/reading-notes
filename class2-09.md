## Reading Notes 09

## Functional Programming Concepts

### What is functional programming?

It is "a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data" - [Wikipedia: Functional programming](https://en.wikipedia.org/wiki/Functional_programming) and [Medium: Concepts of Functional Programming in Javascrip](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa).

### What is a pure function and how do we know if something is a pure function?

It is pure function when [^2]:

- if given the same arguments, it returns the same results
- there is no observable side effects

Pure function, also is referred to as *deterministic* [^2].

### What are the benefits of a pure function?

The benefis of Pure Function according to [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa):

- it is easier to test
- no need to mock anything, and
- unit test pure functions with:
  - "Given a parameter A → expect the function to return value B [^2]"
  - "Given a parameter C → expect the function to return value D [^2]"

### What is immutability?

Immutability means that the data cannot change its after it's created [^2]. When data is ummutable, you cannot change it, howeever, one can create a new object with a new value [^2]. 

### What is Referential transparency?

*'pure functions + immutable data = referential transparency'* - [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

If an expression is referentially transparet, then it can be replaced with its value - or vice, modifying the program/system's behavior.


[^1]: [Wikipedia: Functional programming](https://en.wikipedia.org/wiki/Functional_programming)
[^2]: [Medium: Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

