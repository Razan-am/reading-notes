# **JAVASCRIPT**

## ***Chapter 10: “Error Handling & Debugging”***

### **Order of execution** 
-  scripts are processed in order in which statements are executed, and some tasks cannot complete until another statement or function has been run.

### **Execution contexts**
- `GLOBAL CONTEXT`:code that is in the script, but not in a function.
>There is only one global context in any page.
- `FUNCTION CONTEXT`:code that is being run within a function.
>Each function has its own function context. 

### **VARIABLE SCOPE**
- `GLOBAL SCOPE`:when declared a variable outside a function, `it can be used anywhere because it has global scope`.
- `FUNCTION-LEVEL SCOPE`:when a variable is declared within a function,`it can only be used within that function`.

### **The stack**
- Javascript executed on line of code at a time,and when a statement need a data from another line it will be stack that line before the cureent task.

### **EXECUTION CONTEXT & HOISTING**
- When enters a new execution context, there are two phases
of activity: 
  1. `prepare`:the new scope is created,and the variables, functions, and arguments are created,the value of the this keyword is determined.
  2. `execute`:now it can assign values to variables,reference functions and run their code,execute statements. 

### **Errors**
- `ERROR OBJECTS`:error objects can help you find where your mistakes are and browsers have tools to help you read them.
>It will be appear in the JavaScript console/Error console
of the browser.  
- `TYPES OF ERRORS`:
  1. **Syntax Error**:`SYNTAX IS NOT CORRECT`,this is caused by incorrect use of the rules of the language. It is often the result of a simple typo. 
  2. **ReferenceError**:`VARIABLE DOES NOT EXIST`,this is caused by a variable that is not declared or is out of scope. 
  3. **Type Error**:`VALUE IS UNEXPECTED DATA TYPE`,this is often caused by trying to use an object or method that does not exist. 
   4. **RangeError**:`NUMBER OUTSIDE OF RANGE`,if you call a function using numbers outside of its accepted range. 
   5. **Error**:`GENERIC ERROR OBJECT`,the generic Error object is the template or prototype from which all other error objects are
created.  
   6. **NaN**:`NOT AN ERROR`,if you perform a mathematical operation using a value that is not a number, you end up with the
value of NaN, not a type error. 
   
- `HOW TO DEAL WITH ERRORS`
   1. Debug the scriptt to fix the errors:to track down the source of the error and fix it. 
   2. Handle errors gracefully:you can handle errors gracefully using try, catch,throw, and finally statements. 

- `A DEBUGGING WORKFLOW TECHNIQUES`
  - **Where is the problem?**
  - **What exactly is the problem?**

>The JavaScript console will tell you when there is a problem with a script,where to look for the problem, and what kind of issue it seems to be. 

>In the internet console, the console will show you when there is an
error in your JavaScript. It also displays the line where it became a problem for the interpreter. 

- `DEBUGGING TIPS`
  - Try another browser,some problems are browser specific. 
  - Write numbers to the console so you can see which the items get logged. 
  - Remove parts of code, and strip it down to the minimum you need.
  - Programmers often report finding a solution to a problem while explaining the code to someone else. 
  - SEARCH:stack Overflow is a Q+A site for programmers. 
  - Use the `CODE PLAYGROUNDS`
  - Use the `VALIDATION TOOLS` that can help you try to find errors in your code.
>For JAVASCRIPT `http://www.jslint.com`,,,,`http://www.jshint .com`

- `COMMON ERRORS`
- this is a list of common errors you might find with your scripts.  
    1. `GO BACK TO BASICS`:javaScript is case sensitive so check your capitalization. 
    2. `MISSED/ EXTRA CHARACTERS`:every statement should end in a semicolon. 
    3. `DATA TYPE ISSUES`:using`= `rather than `==` will assign a value to a variable, not check that the values match. 

```<An over all about Error Handling & Debugging>```
- If you understand execution contexts which have two stages and stacks, you are more likely to find the error in your code.
- Debugging is the process of finding errors. It involves a process of deduction.
- The console helps narrow down the area in which the error is located, so you can try to find the exact error.
- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.
- Use them to give your users helpful feedback. 


@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)
