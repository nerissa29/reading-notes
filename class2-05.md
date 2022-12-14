# Reading Notes 05

Ths topic shows us how breaking down the UI in component Hierarchy and figuring out which data needs state and where it needs to live can play an important role in building an app.

## React Docs - Thinking in React

### What is the single responsibility principle and how does it apply to components?

A *single responsibility* principle has each component do one thing. If the idea keeps growing, that component "should be decomposed into smaller subcomponents [^1]".

The screenshot/information below are provided by the article [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html):


<img width="280" alt="image" src="https://user-images.githubusercontent.com/113204667/197222076-d5bb5f93-6025-46ac-ac0f-0b456d39fb85.png">

<img width="347" alt="image" src="https://user-images.githubusercontent.com/113204667/197222151-40c188e4-b161-4ab7-bd02-9278095eab2e.png">

### What does it mean to build a ‘static’ version of your application?

Building a *static version* is a way to implement your app once the component hierarchy has been decided [^1]. It's the same as building components and their subcomponents passing in data using props, but without using *state*. The state is applied during the interactivity phase.

### Once you have a static application, what do you need to add?

Once the static version that renders the app is built, the next step is adding interactivity; this is where the *state* comes in. "Identify The Minimal (but complete) Representation of UI State" will be the next step [^1]. Breaking down pieces of data and figuring out which needs state is essential. 


### What are the three questions you can ask to determine if something is state?

To determine if something is state, ask these three questions from [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html):

- "Is it passed in from a parent via props? If so, it probably isn’t state.[^1]"
- "Does it remain unchanged over time? If so, it probably isn’t state.[^1]"
- "Can you compute it based on any other state or props in your component? If so, it isn’t state.[^1]"
[^1]: [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html)


### How can you identify where state needs to live?

By identifying what piece of data changes or needs to be updated. Examples include input from forms, checkboxes, or text values from search bars. These data change over time and "can't be computed from anything [^1]". The state needs to live inside its parent/grandparents’ components that will be able to pass down the data whenever its child components need it.


## Higher-Order Functions

### What is a “higher-order function”?
The *higher-order function* are functions "that operate on other functions, either by taking them as arguments or by returning them [^2]". *Higher-order function* allows us to either create new functions or change other functions.


### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

The line 2 in the code sample below from [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK) returns the value of the arrow function comparing if the value of m is greater than the value of n.


```
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true

```

### Explain how either map or reduce operates, with regards to higher-order functions

The *map()* returns a new array "by applying a function to all of its elements and building a new array from the returned values[^2]". It will have the same length as the original array, but its contents are now changed depending on the condition/code block of the function applied to it. The *reduce()* is mainly used to compute every single value of the array; it takes "a single element from the array and combines it with the current value [^2]".



[^1]: [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
[^2]: [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)


