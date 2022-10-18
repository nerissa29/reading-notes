# Reading NOtes 2

## React lifecycle

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

According to [Blankenship(2018)](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093), the idagram/image below shows that the *render* happens first before the *componentDidMount*

<img width="498" alt="image" src="https://user-images.githubusercontent.com/113204667/196461883-044317e5-60c6-406d-a479-027f4211e51f.png">

### What is the very first thing to happen in the lifecycle of React?

*Mounting* happens when an instance of the component "is being created and inserted into the DOM[^1]". During Mounting phase, the following occrs in order:

- Constructor
- static
- getDerivedStateFromProps
- render
- componentDidMount
- UNSAFE_componentWillMount

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

Based on the diagram, the following happens in order[^1]:
- constructor
- render
- React updates
- componentDidMount
- componentWillUnmount

### What does componentDidMount do?

Once the component is mounted, the *componentDidMount* will immediately invoked; DOM initialization or network request usually goes here [^1]. [Blankenship(2018)](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093) states in his article that this method is good for setting up subscriptions, while componentWillUnmount() is for unsubscribing.

## React State Vs Props

### What types of things can you pass in the props?

Props can pass data from one component to another; parent component uses props to pass data to its child components[^2]. On the other hand, *state* can only be changed by its own component, and is not available or cannot pass to another component[^3].

### What is the big difference between props and state?

Props are external and is passed into the components, while state is internal - "handled inside" of that component and can only be change by that component itself [^3]. State can be update inside the component, while props are handled and must be updated outside of the component[^3].

### When do we re-render our application?

We re-render our application when there is an update in state or props. We also render child components everytime parent component is rendered or re-rendered[^4].



[^1]: [Blankenship(2018)](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
[^2]: [React Docs: Passing Props to a Component](https://beta.reactjs.org/learn/passing-props-to-a-component)
[^3]: [Web Dev Simplified: React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)
[^4]: [Re-rendering Components in ReactJS](https://www.geeksforgeeks.org/re-rendering-components-in-reactjs/)
