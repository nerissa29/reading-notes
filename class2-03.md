# Reading Notes 3

## React Docs - lists and keys

### What does .map() return?

According to [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map), it creates a new array, "populated with the results of calling a provided function on every element in the calling array".

### If I want to loop through an array and display each value in JSX, how do I do that in React?

The *JSX* "allows embedding any expression in curly braces", which can be used or inline with the map()[^1]. An example would be looping over the array using map(), and assigning those resulting array values/elements into HTML elements by placing them inside the {}[^2].

Below is a screenshot from the article [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html):

<img width="384" alt="image" src="https://user-images.githubusercontent.com/113204667/196720732-cde00040-d3b6-4dae-bc20-bd3a2965643c.png">

<img width="377" alt="image" src="https://user-images.githubusercontent.com/113204667/196720778-7952aaba-cbe5-4dbc-be4b-e1dac5e99108.png">


### Each list item needs a unique ____.

Each list items must have a unique keys. These keys does not need to be global, but keys used within the array must be " unique among their siblings"[^2]. According to the article [React: Lists and Keys](https://reactjs.org/docs/lists-and-keys.html), the same keys can be used when producing two different arrays.

### What is the purpose of a key?

The purpose of the key in React is to identify which items are added, modified, or removed[^2]. It should be given inside the array, when looping over the array, to give the elements their identity.


## The Spread Operator

### What is the spread operator?

The spread operator is useful and an easy way of adding and combining items into the array, or objects; it's also useful in spreading the "array out into a function’s arguments[^3]".

### List 4 things that the spread operator can do.

According to Austin (2019) in his article [How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab), the spread operator '...' can be used in:

- adding arrays/objects
- combining arrays/objects
- using the array as arguments
- adding to state in React

### Give an example of using the spread operator to combine two arrays.


A screenshot from Austin's example in [How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab):

<img width="531" alt="image" src="https://user-images.githubusercontent.com/113204667/196735228-4af57979-e492-4427-8d58-c922d107adad.png">


### Give an example of using the spread operator to add a new item to an array.

Another screenshot from Austin's example in [How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab):


<img width="531" alt="image" src="https://user-images.githubusercontent.com/113204667/196733622-a72993b1-b1fa-446d-8ca7-b407f2912992.png">

### Give an example of using the spread operator to combine two objects into one.

Using the code provided in [How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab), two objects are combined into one:

[How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)




[^1]: [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
[^2]: [React: Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
[^3]: [How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
