# Reading Notes 1

It is critical to understand the flow of data, especially when building web applications and user interface.

## Component-Based Architecture

### What is a “component”?

A component is a "software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities"[^1].


### What are the characteristics of a component?

According to [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm), the characteristics of Components are:

- Reusability 
  - it is designed to be reused in different applications and different situations; some components may also have a specific task
- Replaceable 
  - it can be replaced or substituted with similar components
- Not Content specific
  - it can operate in different contexts and environments
- Extensible
  - to provide new behavior, it can be extended
- Encapsulated
  - it does not expose internal processes details, and it depicts interfaces
- Independent
  - it has minimum dependencies on other components


### What are the advantages of using component-based architecture?

The advantages of using component-based architecture, based on [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm), is as follows:

- Ease of deployment
- Reduced cost
- Ease of Development
- Reusable
- Modification of technical complexity
- Reliability
- System maintenance and evolution
- Independent


## What is Props and How to Use it in React

### What is “props” short for?

*Props* is short for *properties* which is used for "passing data from one component to another"[^2]. Props' data are passed in one-way - from parent to child; one way is known as *unidirectional flow*. Also, the data coming from the parent is read-only, child-components must not change this data.


### How are props used in React?

**Props in React (According to [What is “Props” and how to use it in React?](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)):**

- define the attribute and its values
- using props, pass this to child components
- render the Props Data

Example[^2]:

```
class ParentComponent extends Component {  
  render() {
    return (
      <h1>
        I'm the parent component.
        <ChildComponent />
      </h1>
    );
  }
}
```


### What is the flow of props?

Props data flow in one-way, from parent to child; it is also known as the unidirectional flow.


## Things I want to know more about
I want to see this information being used or applied in a code.


[^1]: [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)
[^2]: [What is “Props” and how to use it in React?](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)




