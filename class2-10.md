## Reading Notes 10

### Understanding the JavaScript Call Stack

#### What is a ‘call’?

The call stack is used everytime a function is invoked, each done "one at a time, from top to bottom [^1]". The call stack is synchronous - [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

#### How many ‘calls’ can happen at once?

The function execution is only done one at a time.

#### What does LIFO mean?

LIFO stands for Last In, First Out, a data structure that the call stack uses, as it temporary store and manage function calls [^1].

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
   
   
The function *sayHi()* didn't crossed the stack until it is called/invoked in line 24. Lines 20-22 are only a function declaration - function sayHi(name){...}. Line 24 is where we declare a variable *greetings1* and assign it to the evaluated result of ***invoking the function sayHi()*** passing in the arguments 'Ella'.

#### What causes a Stack Overflow?

A stack overflow happens when there is an infinite loop, or a recursive call that does nothave an exit point/condition [^1].


### JavaScript error messages

#### What is a ‘reference error’?

A reference error is when you use a variable that is not defined or declared[^2].

#### What is a ‘syntax error’?

Syntax errors are errors that cannot be parse; a good example would be missing a semi-colon or having trailing comma or spaces [^2].

#### What is a ‘range error’?

Range errors exist when manipulating data or objects, giving "it an invalid length" - [^2]: [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).

#### What is a ‘type error’?

Type errors occur when "the types (number, string and so on) you are trying to use or access are incompatible" - [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).

#### What is a breakpoint?

A breakpoit is achieved by placing "a debugger statement in your code in the line you want to break [^2]".
[
](https://miro.medium.com/max/1100/1*yhFA4njFS7JCRVZPzvDU-A.png)




[^1]: [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)
[^2]: [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

