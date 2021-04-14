# **JAVASCRIPT**

1. **How to write a script for a web page** 

**```There is  three languages that are used to create web pages:```**
**HTML, CSS, and JavaScript.** 

With keeping the three languages in separate files, HTML page is linking to CSS and JavaScript files.Each language forms a different purpose.

- **<html>**: CONTENT LAYER (. html files)
- **{css}** : PRESENTATION LAYE (. css files)  
- **j avascri pt()**: BEHAVIOR LAYER (.js files)

These three layers form the basis of a popular approach to building web pages called progressive enhancement. 

- `HTML ONLY` :The HTML layer allows you to focus on the most important thing about your site:
`its content`. 
- `HTML+CSS` :The CSS rules works on how `the page looks`
away from the content itself.
- `HTML+CSS+JAVASCRIPT` :The JavaScript is added last
and enhances the users experience of `interacting with the site`.  

2. **CREATING A BASIC JAVASCRIPT** 

JavaScript is written in plain text, just like HTML and CSS,so you do not need any new tools to write a script.And to link it with the HTML :

1. Create a folder to put the javascript file into it `Ex; add-content . j s `
2. Use the HTML `<script>` element to tell the browser it is coming across a script. 

`<body>`

`<hl>Constructive &amp ; Co. </ hl>`

`<script src="js/ add-content.js"></ script>`

`<p>For all orders and i nquiries please cal l`

`<em>SSS-3344</ em></ p>`

`</ body>`

3. **Applying objects and methods**

It will be applied using `document.write(object)`
its  usually work with the conditions command.


**JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML**

+ It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension. 

+ The HTML <script> element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the <link> element can be used to load a CSS file). 

+ If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created.


>Example of the Javascript commands:
var today= new Date();
var hourNow = today.getHours();
var greeting;
if (hourNow > 18) {
greeting= 'Good evening!';
else if (hourNow > 12) {
greeting = ' Good afternoon!';
else if (hourNow > 0) {
greeting = 'Good morni ng!';
else {
greeting = 'Welcome! ' ;
document .write( ' <h3>' +greeting + ' </ h3> '); 

3. **Reading and writting JavaScript.**

+ **STATEMENTS** :Statement are instructionsand each one starts on a new line, and it can be organized into code blocks by surround it with curly braces ({});these are known as code blocks.

+ **COMMENTS** :You should write comments to explain what your code does. 
There is two ways to write comments:
1. Using `/* */` and its for multi-line comments .
2. Using `//` and its for single-line comments.

+ **A VARIABLE** :A data that is temporarily
store information it needs to do a certine job.

>For example: 
var variable name = 'variable value';
var age = '35';

+ **DATA TYPES** : JavaScript distinguishes between numbers,
strings, and true or false values known as
Booleans. 

  - NUMERIC DATA TYPE :0.75
  - STRING DATA TYPE : 'Hi'
  - BOOLEAN DATA TYPE : True or false

+ **USING A VARIABLE TO STORE A NUMBER** :

>For exampels :
var price =  5;
var quantity = 14;

+ **USING A VARIABLE TO STORE A STRING** :

>For example :
var username = 'Molly';
var message =  'See our upcoming range';

+ **USING QUOTES INSIDE A STRING** :

>For exampel:
var title = "Molly's Special Offers" ;
var message = '<a href=\"sale .html\">25% offl</a>' 

+ **USING A VARIABLE TO STORE A BOOLEAN**

>For exampel:
var i nStock = true;
var shipping = = false;

+ **SHORTHAND FOR CREATING VARIABLES** :

>For exampel:
var price = 5;
var quantity = 14;
var total = price * quantity;



**References:**

@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)
