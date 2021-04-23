# **JAVASCRIPT**

### **Decisions and loops**

- Creating and controlling the flow of data in your scripts  `(Codes)` to handle different situations,making the browser be able to runs different code in different situations.

- Scripts often need to behave differently depending upon how the user interacts with the web page and/or the browser window itself. To determine which path to take, programmers often rely upon the following three concepts: 

1. **EVALUATIONS :**You can analyze values in your scripts to determine whether or note they match expected results. 


2. **DECISIONS :**The results from evaluations you can decide which path your script should go down.


3. **LOOPS :**There are also many occasions where you will want to perform the same set of steps repeatedly

### ***Decisions making***
In the script there is sveral places in charge in determine wich line of code should run next.

>For examples :
There is decesion that must be made so the code can take one of the different pathes and each one of these pathes are made of set of tasks.Thats means for each situation you have to write different code.
In order to determine wich path to take you'll set a condition and depending on the result the path will be choosen.



#### **Comparison operators:**

there are two componant to decision :

1. **Evaluating condition:** an expression is evaluated which is returns avalue .

2. **Conditional statments:** aconditional statment says what to do in a given situation.

#### **Evaluating condition**
- You can evaluate a situation by comapring one value in the script to what you expect it might be .

- The result in the boolean will be eather  `true or false ` , using a comparison operators such as :
  - Greater than (>):checks if the number on the left is greater than the number on the right 

  - Less than (<):checks if the number on the left is less than the number on the right

  - Greater than or equal to (>=) :checks if the number on the left is greater than or equal to the number on the right.

  - Less than or equal to (<=):checks if the number on the left is less than or equal to the number on the right.

  - Equal to ( == ):the operator compare two values (numbers, strings,boolean) to see if they are the same .

  - Not equal to (!=):the operator compare two values (numbers, strings,boolean) to see if they are not the same .

  - Strict equal to (===):the operator compare two values to check if that both the datatype and the value are the same. 

  - Strict not equal to (!===):the operator compare two values to check if that both the datatype and the value are not the same.
 
>For example:

![Image](https://i.stack.imgur.com/kin2r.jpg)


#### **Logical operators:**
Comparision operators returns a single value (True or false),the logical operators allows you to compare the result of more than one comparision operator .

![image](https://res.cloudinary.com/practicaldev/image/fetch/s--iAbnVv87--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://cl.ly/7d9cf8370380/Image%25202018-11-15%2520at%25209.59.47%2520AM.png)

#### **If Statments:**

The if statment checks and evaluates the result of a condition with  `true or false `.

>Example :
var pass = 50;
var score = 75;
var msg;
// Pass mark
// Current score
// Message
// Select message to write based on score
if (score >= pass) {
msg = 'Congratulations, you passed!';
} else {
msg = 'Have another go!'; 

#### **TYPE COERCION & WEAK TYPING:**

- Javascript using data types for each operation 
   - DATA TYPE PURPOSE

|         Datatype               |      Purpose   |
|--------------------------------|----------------|
|string                          |Text            |
|number                          |Number          |
|Boolean                         |true or false   |
|nul 1                           |Empty value     |
|undefined                       | Variable has been declared but not yet assigned a value |

>If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error. 

### ***Loops***

- Loops are used when we have repeated condition

The commoun types of loops:
  1. **While :**when you don't know how many times the code should run 
  2. **For :**if you need to run a code in a specific numbers of times 


- **While loop:**

![image](https://study.com/cimages/multimages/16/cb730cff-275e-4ff8-92c1-a309f5d1ff41_c_loop_flow.png)

>For example
var i = l ;
var msg = ' ' ;
// Set counter to 1
// Message
// Store 5 times tabl e in a variable

>while (i < 10) {
msg += i + ' x 5 = ' + (i * 5) + '<br I>';
i++; 
{

- **For loop:**

![image](https://i.pinimg.com/originals/fa/69/f6/fa69f6c681b2baa417be37dedc737bba.gif)

- For loop componants:
  - Initialization:creating the counter of the loop 
>var i = 0;
  - Condition:the loop continuing to run depending on the condition 
>i < 10;
  - Updated (increments):the loop keep running the statement in between the curly braces such as adding one to the counter
>i++

### EXAMPLE of using DECISIONS & LOOPS together in Javascript 

>// Unit of table
var table = 3;
// Type of calculation (defaults to addition)
var operator= 'addition';
// Set counter to 1
var i = 1;
// Message
var msg = ' ' ;

>// If the operator variable says addition
if (operator=== 'addition')
// While counter is less than 11
while (i < 11) {
  Calculation
msg += i + ' + ' + table + ' = ' + (i +table)+ '<br I>'; 
// Add 1 to the counter
i++;
}
// Otherwise
else {
// Whi le counter is less than 11
while ( i < 11) {
  // Calculation
msg += i + ' x ' + table + ' = ' + (i *table) + '<br I> '; 
// Add 1 to the counter
i++;
 }

>}


>// Write the message into the page

**Overall about DECISIONS & LOOPS**
+ Conditional statements allow your code to make
decisions about what to do next.
+ Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.
+ Logical operators allow you to combine more than one
set of comparison operators.
+ if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.

+ Data types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loop: for, while, and
do ... while. Each repeats a set of statements.





**References:**

@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)



 