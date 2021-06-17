# In memory storage

## Understanding the JavaScript Call Stack
1. What is a ‘call’?

    a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

2. How many ‘calls’ can happen at once?

    it can only do one thing at a time.

3. What does LIFO mean?

    Last In, First Out, which basically means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
    
    ```
    function firstFunction(){
    throw new Error('Stack Trace Error');
    }

    function secondFunction(){
        firstFunction();
    }

    function thirdFunction(){
        secondFunction();
    }

    thirdFunction();
    ```
    

5. What causes a Stack Overflow?

    when a function that calls itself without an exit point.


## JavaScript error messages
1. What is a ‘refrence error’?

    This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

2. What is a ‘syntax error’?
    
    This error occurs when you have something that cannot be parsed in terms of syntax. 

3. What is a ‘range error’?

    This error occurs when a value is not in the set or range of allowed values.


4. What is a ‘tyep error’?

     This error occurs when the types (number, string and so on) you are trying to use or access are incompatible.

5. What is a breakpoint?

    It is used when debugging, it stops the compiler at a certain line, giving the values for all the variables, in order to fix a bug in the application.

6. What does the word ‘debugger’ do in your code?

    Debugger is use to stops the execution of code, bu using breakpoint.