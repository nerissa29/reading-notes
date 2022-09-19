## Reading Notes 06

## How would you describe an object to a non-technical friend you grew up with?

An object is created by defining a variable and initializing a value to that variable[^1]. It's like a water bottle, where the bottle acts as the variable (since it’s the placeholder of the water), and the water acts as its value.

## What are some advantages to creating object literals?
Object literal, according to MDN web docs, are lists “of zero or more pairs of property names and associated values of an object, enclosed in curly braces ({})”[^2]:
```
const sales = "BMW";

function carTypes(name) {
  return name === "Honda" ? name : `Sorry, we don't sell ${name}.`;
}

const car = {
  myCar: "Toyota",
  getCar: carTypes("Honda"),
  special: sales,
};

console.log(car.myCar); // Toyota
console.log(car.getCar); // Honda
console.log(car.special); // BMW
```
Object literals provide a shorter/smaller syntax for calling the functions and are usually an array of key:value pairs. The *colon ‘ : ’* is used to separate the object keys and their values. It is useful when used along with the constructors. Object literals can also increase its reusability, and are most useful when storing many different values under the same key.

## How do objects differ from arrays?
The objects are mutable and serve as a placeholder used to store sets of data. Arrays are also mutable and used to store lists/sets of values. The built-in method isArray() is used to determine if the object is an array. Arrays don’t have keys / key:values pair, unlike the object literals..

## Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
*Bracket notation* is another way to access object properties. It is similar to accessing array elements, except that instead of using index, the name (or key) associated to the values are used to select an item[^1].
*Example using our objects *car* above:
car[myCar]  
car[getCar]  
car[special]  

## Evaluate the code below. What does the term this refer to and what is the advantage to using this?

```
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

```

The *this* keywor refers to the object name *dog*. The *this.name* is same as *dog.name*.

## Introduction to the DOM

## What is the DOM?

The *DOM (Document Object Model)* "is a programming interface for web documents" representing the page, allowing programs to change the structure, content, and style of the document[^3].

## Briefly describe the relationship between the DOM and JavaScript.

*DOM* "can be modified with a scripting language such as JavaScript"; an example would be using the *querySelectorAll* to select all the *p* elements[^3]:

```
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
```



References:
[^1]: [JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)
[^2]:  [Literal](  https://developer.mozilla.org/en-US/docs/Glossary/Literal))
[^3]: Introduction to the DOM(https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

