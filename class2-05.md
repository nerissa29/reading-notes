# Reading Notes 05

## React Docs - Thinking in React

### What is the single responsibility principle and how does it apply to components?

A *single responsibility* principle has each component do one thing. If the idea keeps growing, that component "should be decomposed into smaller subcomponents [^1]".

The screenshot/information below are provided by the article [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html):


<img width="280" alt="image" src="https://user-images.githubusercontent.com/113204667/197222076-d5bb5f93-6025-46ac-ac0f-0b456d39fb85.png">

<img width="347" alt="image" src="https://user-images.githubusercontent.com/113204667/197222151-40c188e4-b161-4ab7-bd02-9278095eab2e.png">

### What does it mean to build a ‘static’ version of your application?

Building a *static version* is a way to implement your app once the component hierarchy has been decided[^1]. It's same as building components and its subcomponents passing in data using props, but without using *state*. State is applied during interactivity phase.

### Once you have a static application, what do you need to add?

Once the static version that renders the app is built, next step is adding interactivity; this is where the *state* comes in. "Identify The Minimal (but complete) Representation Of UI State" will be the next step [^1]. Breaking down pieces of data and figuring out which needs state is important, ask these three questions from [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html):

- "Is it passed in from a parent via props? If so, it probably isn’t state.[^1]"
- "Does it remain unchanged over time? If so, it probably isn’t state.[^1]"
- "Can you compute it based on any other state or props in your component? If so, it isn’t state.[^1]"


[^1]: [React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html)


