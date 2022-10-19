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




[^1]: [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
[^2]: [React: Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
