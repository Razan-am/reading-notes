## **Understanding the JavaScript Call Stack**

### ***What is a `call`?***

- It's means that we invocting the function by calling it 

### ***How many `calls` can happen at once?***

- It's  is done, one at a time, from top to bottom. It means the call stack is synchronous.

### ***What does LIFO mean?***

- It's stand for the principle of `Last In, First Out`, which it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### ***Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.***

- ![Image](../imag/stack.PNG)

### ***What causes a Stack Overflow?***

- It's happened when there is a recursive function `a function that calls itself` without an exit point.

-------------------------------------------------

## **JavaScript error messages**

### ***What is a `refrence error`?***

- It's means that when you try to use a variable that is not yet declared you get this type os errors.

### ***What is a `syntax error`?***

- It's means  when you have something that cannot be parsed in terms of syntax.

### ***What is a `range error`?***

- It's means when you  invalid length to an object with some kind of length.

### ***What is a `tyep error`?***

- It's means when the types `number, string .....` you are trying to use or access are incompatible.

### ***What is a breakpoint?***

- It's means putting a debugger statement in your code in the line you want to break.

### ***What does the word `debugger` do in your code?***


- Debugging is the process of detecting and removing of existing and potential errors in the code by using the `console.log()` the variables you want to check.


----------------------------------------------------------------------

**References:**

@By Charles Freeborn /[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

@By Diogo Spínola/[JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)