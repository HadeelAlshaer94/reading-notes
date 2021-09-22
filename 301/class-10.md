# Code 301 - Intermediate Software Development

# Memory storage

![call](https://miro.medium.com/max/638/1*CCHexfHNCNo-f8aw3rbRew.jpeg)

## What is a ‘call’?
At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

## How many ‘calls’ can happen at once?
The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

## What does LIFO mean?
LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### an example of a call stack and the functions that would need to be invoked to generate that call stack.
![call](https://miro.medium.com/max/1400/1*rJ2sh-q1deQGGGVG5gYyIQ.png)

## What causes a stack overflow?
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

----------------------------------
# JavaScript error messages


## What is a ‘refrence error’?
An #REF error (the “ref” stands for reference) is the message Excel displays when a formula references a cell that no longer exists, usually 
 by deleting cells that a formula is referring to.

## What is a ‘syntax error’?
An exception caused by the incorrect use of a pre-defined syntax. Syntax errors are detected while compiling or parsing source code. For example, if you leave off a closing brace ( } ) when defining a JavaScript function, you trigger a syntax error.   

## What is a ‘range error’?
Description. A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value. This can be encountered when: passing a value that is not one of the allowed string values to String.

## What is a ‘type error’?
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

## What is a breakpoint?
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values. In this example the breakpoint will point stop when the index reaches 40.

![deb](https://www.edureka.co/blog/wp-content/uploads/2019/08/debuuging-steps-528x294.png)
## What does the word ‘debugger’ do in your code?
Debuggers allow users to halt the execution of the program, examine the values of variables, step execution of the program line by line, and set breakpoints on lines or specific functions that, when hit, will halt execution of the program at that spot.