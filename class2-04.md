# Reading Notes 04

## React Docs - Forms

### What is a ‘Controlled Component’?

Controlled Components are input form elements in which the form's data or values are handled by it's own component's state; it is controlled by React[^1].

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

In controlled compoent, the user input values are always controlled by React, as the user types, the event that target that value will run, updating the React state[^1]. According to [React Docs: Forms](https://reactjs.org/docs/forms.html), with "a controlled component, the input’s value is always driven by the React state".


### How do we target what the user is entering if we have an event handler on an input field?

Form elements like *input* maintains and updates their own state based on the user input. Th event handler on the inout field will then run "on every keystroke to update the React state[^1]"; it will update te displayed value as the user types.

## The Conditional (Ternary) Operator Explained

### Why would we use a ternary operator?

The ternary operator shortens the if-else statement into one line (Morelli, 2017).

### Rewrite the following statement using a ternary statement:

```
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

Using Ternary operator:
x===y ? console.log(true) : console.log(false)

Note that the 5 line of code in the original if-else statement has been shorten into one line of code using the ternary operator.

#### Resources
Morelli, B. (2017, December 18). *JavaScript - the conditional(ternary) operator explained*. Codeburst. https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff
[^1]: [React Docs: Forms](https://reactjs.org/docs/forms.html)



