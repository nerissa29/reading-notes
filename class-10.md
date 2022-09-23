## Reading Notes 10

### Readings: Debugging

#### Name some key differences between a Syntax Error and a Logic Error.

An example of syntax errors causing the program not to run or work properly is spelling errors. An error message may be provided and can be fixed “with the right tools and know what the error messages mean![^1]”. Logic errors, on the other hand, are errors where the syntax is correct, “but the code is not what you intended it to be[^1]”. It runs correctly, but the result isn’t correct.

#### List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.

I encountered misplacing variables, placing and initializing them inside the for loops; this is not ideal when that variable is supposed to increment, like a sum variable. I also experienced sitting for hours just to find out that my inner loop is missing a j++, causing the page to run into an infinite loop, crashing the site. Sometimes, I do encounter logic errors, especially when I don’t understand what the problem is asking.

#### How will this topic continue to influence your long term goals?
Syntax and logic errors are part of being a developer. There will always be a point where I will encounter these two over and over again. It is also part of a learning process. 

### The JavaScript Debugger.

#### How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

As described in MDN, the JavaScript debugger allows us to see the value of the variables. It alse sets breakpoints, placed in “code that you want to pause execution and identify the problems that prevent your code from executing properly”[^2].

To open[^2]:

- Keyboard: Ctrl + Shift + I, except
  - Internet Explorer and Edge: F12
  - macOS: ⌘ + ⌥ + I

- Menu bar:
  - Firefox: Menu




[^1]: [What went wrong? Troubleshooting JavaScript]( https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_went_wrong)
[^2]: [What are browser developer tools?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools#the_javascript_debugger)

