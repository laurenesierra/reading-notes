# The Call Stack

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

[The Call Stack Defined MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call). This means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

Temporarily store: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.

Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

Think of yourself standing on a queue, in a grocery store cash point. You can only be attended to after the person in front of you have been attended to. That’s synchronous.

This is what we mean by “manage function invocation”.

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error. 

__The key takeaways from the call stack are:__
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

[Understanding the Javascript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

# Javascript Error Meassages

### Types or Error Messages:

- Reference errors:


This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

Syntax errors:
I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

Range errors:
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

Type errors
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.


[Javascript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

[Javascript Errors Refernence MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

[<----Back Home](../README.md)