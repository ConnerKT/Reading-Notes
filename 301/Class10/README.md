# In Memory Storage Notes

This topic is important to me because I want to be able to use error handling correctly and use in memory storage well.

## [Retrospective 10](https://connerkt.github.io/Reading-Notes/301/Class10/Retro10)

## References

[JS Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4).

[JS Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c).

[Error References MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors).

## JavaScript Call Stack

The JS engine, is a single-threaded interpreter comprising of a heap and a single call stack.

Call stack is used for function invocation(call).

Since the call stack is single, functions execution is done one at a time. Top to bottom. The call stack is synchronous.

Understanding the call stack is vital to Asynchronous programming.

In Asynchronous JS, we have a callback function, an event loop and a task queue.

A **Call Stack** is a data structure that uses Last In, First Out principe to temporarily store and manage function calls.

Last In, First Out (LIFO) - Means that the last function that gets pushed into the stack is the first to be pop out when the function returns.

When a function is invoked, the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it pops out.

A **Stack Overflow** occurs when there is a recursive function(a function that calls itself) without an exit point.

IN SUMMARY:
Javascript is single threaded- only one at a time.
Code execution is synchronous.
A function invocation creates a stack frame that occupies a temporary memory.
Works as a LIFO.

### In Memory Storage Questions

1. What is a ‘call’?
2. How many ‘calls’ can happen at once?
3. What does LIFO mean?
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
5. What causes a Stack Overflow?

### In Memory Storage Answers

1. A call is when you execute a function
2. One
3. Last in, First Out
4. https://share.sketchpad.app/23/a43-0ca0-4bbc36.png
5. When there is a recursive function without an exit point.

## JavaScript Error Messages

Error messages are given to us in coding to help diagnosis whats wrong with our code!

**Reference Errors** -When you try to use a variable that is not yet declared. Or don't give it a let,const,var.

**Syntax Error** - This occurs when you have something that cannot be parsed in terms of syntax.

**Range Errors** - Trying to manipulate an object with an length and giving it an invalid length.

**Type Errors** - This shows up when the types (number,string etc) you are trying to use or access are incompatible , like using a property of an undefined type of variable.

To debug your code, you can console.log your code to figure out what you want.

You can also use your debugging tools that come with your browser to select breakpoints and more.

### JS Error Messages Questions

1. What is a ‘reference error’?
2. What is a ‘syntax error’?
3. What is a ‘range error’?
4. What is a ‘type error’?
5. What is a breakpoint?
6. What does the word ‘debugger’ do in your code?

### JS Error Messages Answers

1. When you use a variable that is not declared yet.
2. When you have something that cannot be parsed.
3. When you manipulate an object with a length, and give it an invalid length.
4. When the type you are using are incompatible.
5. A breakpoint is something you can put in your code to stop if a condition is valid. It breaks the code there.
6. It stops the execution of JS and calls the debugger.

## Things I want to know more about

I want to know more about the call stacks, and how it changes with the languages you use.

I want to know how powerful a language can be if it can use more than one thread.
