## Reading Notes 10

### Understanding the JavaScript Call Stack

#### What is a ‘call’?

The call stack is used every time a function is invoked, each done "one at a time, from top to bottom [^1]". The call stack is synchronous - [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

#### How many ‘calls’ can happen at once?

The function execution is only done one at a time.

#### What does LIFO mean?

LIFO stands for Last In, First Out, a data structure that the call stack uses to store and manage function calls temporarily [^1].

#### Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.


function sayHi(name) {
  console.log(`Greetings to you ${name}!`);
}

const greetings1 = sayHi('Ella');



sayHi
_________________
global
_________________
   callstack
   
   
The function *sayHi()* doesn’t cross the stack until it is called/invoked in line 24. Lines 20-22 are only a function declaration - function sayHi(name){...}. Line 24 is where we declare a variable *greetings1* and assign it to the evaluated result of ***invoking the function sayHi()*** passing in the arguments 'Ella'.

#### What causes a Stack Overflow?

A stack overflow happens when there is an infinite loop or a recursive call that does not have an exit point/condition [^1].


### JavaScript error messages

#### What is a ‘reference error’?

A reference error is when you use a variable that is not defined or declared [^2].

#### What is a ‘syntax error’?

Syntax errors cannot be parsed; a good example would be missing a semi-colon or having trailing commas or spaces [^2].

#### What is a ‘range error’?

Range errors exist when manipulating data or objects, giving "it an invalid length" - [^2]: [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).

#### What is a ‘type error’?

Type errors occur when "the types (number, string, and so on) you are trying to use or access are incompatible" - [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).

#### What is a breakpoint?

A breakpoint is achieved by placing "a debugger statement in your code in the line you want to break [^2]". An example is an image below, adapted from [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c):

<img width="537" alt="image" src="https://user-images.githubusercontent.com/113204667/200213400-6f8fc8da-5617-4b3c-81c6-b69a5f902ec7.png">


#### What does the word ‘debugger’ do in your code?

A debugger "stops the execution of JavaScript [^3]".


[^1]: [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)
[^2]: [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
[^3]: [JavaScript Debugging](https://www.w3schools.com/js/js_debugging.asp#:~:text=The%20debugger%20keyword%20stops%20the,debugger%20statement%20has%20no%20effect.)
