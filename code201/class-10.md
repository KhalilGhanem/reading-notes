# JS Debugging
Debugging is the process of finding errors. It involves a 
process of deduction. 

## Execution Contexts
The JavaScript interpreter uses the concept of execution contexts.

Execution Contexts Types:
* Global Contexts:Code that is in the script, but not in a function. There is only one global context in any page.
* Function Contexts:Code that is being run within a function. Each function has its own function context. 


JavaScript interpreter Run the code line by line , and the current statment call another function, the interpreter stacks the new function on teh top of the current line.

Each time a script enters a new execution context, there are two phases of activity: 
1. Prepare: new scope ,Variables, functions, and arguments are created. 
2. Excute: assign values to variables, Execute statements.

hoisting: taking all of the variables and functions and hoisting them to the top of the execution context.

## Errors:
When a statment generates an error, it throws an exception and the interpreter stops and looks for exception-handling code.

We can use some statements to handle the error:
* TRY
* CATCH
* FINALLY 
```
try { 
II Try to execute this code 
} catch (exception) { 
II If there is an exception, run this code 
} finally { 
II This always gets executed 
}

```

### Error objects 

* Error objects can help us find where our mistakes are and the console help us to read those errors.
* When an Error object is created, it will contain the following properties: 
  * name
  * message
  * file number
  * line number
* built-in error objects types:
  * Error
  * Syntax Error 
  * Ref erenceError
  * TypeError
  * Range Error
  * URI Error 
  * Eval Error 

## How to deal with errors:
1. Debug the script.
2. Handel errors.