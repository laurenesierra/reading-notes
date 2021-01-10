
# Error Handling and Debugging

How code can deal with potential errors gracefully. lol


### Order of Execution:

In order to find the source of an error, it helps to know how scripts are processed. Some tasks can not be complete until others are run.

### Execution Contexts and Variable Scope:

There is one global execution context. Each function creates a new execution context.  They corrispond to variable scope.

Execution Context:
- Global Context
(Code in the script but not in a function)
- Function Context
(Code that is being run within a function)
- Eval Context
(Text is executed like code in an internal function)


Variable Scope:
- Global Scope
(If a variable is declared outside a function, it can be used anywhere because it has a global scope. If you do not use the var keyword when creating a variable. it is place within a global scope.)
- Function-Level Scope
(When a variable is declared within a function, it can be used within that function.)


The Stack:

The Javascript interpreter processes one line of code at a time. When a new statement needs data from another function, it stacks (or piles) the new function on top of the current task.
 
 Execution Context and Hoisting:

 Each time a script enters a new execution context, there are two phases of activity:

 1. Prepare
 - The new scope is created.
 - Variables, functions and arguments are created.

 1. Execution
 - Now it can assign value to variables.
 - It can reference functions and run their code.
 - Execute statements.

 Understanding Scope:

 In the interpriter, each execution context has it's own variables object.  It holds the variables, functions and parameters available within it. Each execution context can also access it's parent's variables project.

 Understanding Errors:

 If a Javascript statement detects an error, then it throws an _exception_. At that point, the interpreter stops and looks for exception-handling code.

 Error Objects:

 These can help you find where your mistakes are. Browsers have tools to help you read them.

 ## Debugging Workflow:


Debugging is about deduction: eliminating potential causes for error.  

1. Look at the error message
1. Check how far the script is running (write messages in console)
1. Use breakpoints to determine where things are going wrong.
1. Check to make sure the variables around them have the values you would expect them to.
1. Break down parts of the code to test smaller pieces of the functionality.
1. Check the parameters for a function or the number of items in an array.

Be prepared to repeat the process again once you are finished!

Handling Exceptions:

If you feel like your code might fail use:
1. Try
1. Catch
1. Finally







[<----Back to Home](../README.md)