# **HTML & CSS**
Design and Build Websites

## Contents:

- ### **Chapter 1 :Introduction** 

**```In order to teach you about creating web pages,
this book is divided into three sections:```**
 
+ **HTML** :HTML is used to create web pages. You will see that you start by writing down the words you want to appear
on your page.

+ **CSS** :CSS uses rules to enable you to control the styling and layout of web pages.fall into one of two categories:


  1. `Presentation`:It's about how to control things like the color of text, the fonts you want to use...etc. 

  2. `Layout`: How to control where the different elements               are positioned on the screen

+ **Practical** :It's some helpful information that will assist you in building better websites.

**```Before starting we need to know the differents ways that you can access to web:```**

+ **Browsers** :People access websites using software called a web browser, such as Chrome. 
+ **Web Servers** :When ask your browser for a web page, the request is sent across the Internet to a special
computer known as `a web server` which hosts the website.
+ **Screen readers** :Screen readers are programs that read out the contents of a computer screen to a user.


<img src="images/Capture.PNG" width="200" height="250"/>
<img src="images/Capture1.PNG" width="200" height="250"/>


### So an overall the websites are being built using HTML and CSS,so how these worked ?

+ HTML pages are text documents.
+ HTML uses tags (characters that sit inside angled brackets) to give the information they surround special meaning.
+ Tags are often referred to as elements.
+ Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.
+ Opening tags can carry attributes, which tell us more
about the content of that element.
+ Attributes require a name and a value.
+ To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.


- ### **Chapter 8:Extra Markup**


- ***DOCTYPES***:There are a several versions of HTML, each web page should begin with a `DOCTYPE` declaration to tell a browser which version of HTML the page is using 

- ***Comments in HTML***:If you add a comment to your code it will not be visible in the user's browser, you can add the text between these characters `<!-- -->`.

- ***ID Attribute***:It is used to uniquely identify an element
from other elements,every HTML element can carry
the id,and its value should start with a letter or an underscore (not a number or any other character) like this
 `<p id="pullquote">`

>it's used so that in CSS the element with a
unique identity allows you to style it differently than any other instance of the same element on the page.

------------------------------------------------------------

  - ***Class Attribute***:It is used as an a way to identify several elements as being different from the other elements.
`For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements`
using this `<p class="important">`

  - ***Block Elements***:Some elements will always appear to start on a new line in the browser window. These are
known as block level elements.

>Examples of block elements are `<h1>, <p>, <ul>, and <li>`.

`<h1>Hiroshi Sugimoto</h1>`

`<p>The dates for the ORIGIN OF ART exhibition are as       follows:</p>`

`<ul> `

 ` <li>`

   `  Science: 21 Nov - 20 Feb 2010/11`

 ` </li>`

 `</ul>`


- ***Inline Elements***:Used to appear the elements are continuing on the same line as their neighbouring elements.

>Examples of inline elements are `<a>, <b>, <em>, and <img>.`

- ***Grouping Text & Elements In a Block `<div>`***:Used to
group a set of elements together in one block-level box.

>For example, you might create a `<div>` element to contain all of the elements for the header of your site (the logo and the navigation)
`<div id="header">`

`<img src="images/logo.gif" alt="Anish Kapoor" />`

`<ul>`

 `<li><a href="index.html">Home</a></li>`

 `<li><a href="biography.html">Biography</a></li>`

 `<li><a href="works.html">Works</a></li>`

 `<li><a href="contact.html">Contact</a></li>`

`</ul>`

`</div><!-- end of header -->`


- ***Grouping Text & Elements Inline `<span>`**:
The `<span> `element acts like an inline equivalent of the `<div>` element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text
2. Contain a number of inline
elements
>The most common reason whypeople use <span> elements is so that they can control the appearance of the content of these elements using CSS.

 `<span class="gallery">Tate Modern</span>` 

 - ***IFrames `<iframe>`***: An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.

`<iframe`

`width="450"`

`height="350"`

`src="http://maps.google.co.uk/maps?q=moma+new+york`

`&amp;output=embed">`

`</iframe>`

>**src**:The src attribute specifies the URL of the page to show in the frame.
**height**:The height attribute specifies the height of the iframe in pixels.
**width**:The width attribute specifies the width of the iframe in pixels
**scrolling**:The scrolling attribute will not be supported in HTML5
**frameborder**:The frameborder attribute will not be supported in HTML5.

-----------------------------------------------------------

- **Information About Your Pages**

**`<meta>`**
The <meta> element lives inside the <head> element and
contains information about that web page.And it is not visible to users.

>For example:

`<head>`

 `<title>Information About Your Pages</title>`

 `<meta name="description"`

 `content="An Essay on Installation Art" />`

 `<meta name="keywords"`

 `content="installation, art, opinion" />`

 `<meta name="robots"`

 `content="nofollow" />`

 `<meta http-equiv="author"`

 `content="Jon Duckett" />`

 `<meta http-equiv="pragma"`

 `content="no-cache" />`
 
 `<meta http-equiv="expires"`

 `content="Fri, 04 Apr 2014 23:59:59 GMT" />`
 
`</head>`


### Overall abou extra markup:

+ DOCTYPES tell browsers which version of HTML you are using.
+ You can add comments to your code between the <!-- and --> markers.
+ The id and class attributes allow you to identify particular elements.
+ The <div> and <span> elements allow you to group
block-level and inline elements together.
+ <iframes> cut windows into your web pages through
which other pages can be displayed.
+ The <meta> tag allows you to supply all kinds of
information about your web page.
+ Escape characters are used to include special
characters in your pages such as <, >, and ©.

### An overall example of extra markup:

`<!DOCTYPE html PUBLIC`

`"-//W3C//DTD HTML 4.01 Transitional//EN"`

`"http://www.w3.org/TR/html4/loose.dtd">`

`<html>`

`<head>`

 `<meta name="description" content="Telephone, email`

 `and directions for The Art Bookshop, London, UK" />`

 `<title>Contact The Art Bookshop, London UK</title>`

`</head>`

`<body>`

 `<div id="header">`

 `<h1>The Art Book Shop</h1>`

 `<ul>`

 `<li><a href="index.html">home</a></li>`

 `<li><a href="index.html">new publications</a>`

 `</li>`

 `<li class="current-page">`

 `<a href="index.html">contact</a></li>`

 `</ul>`

 `</div><!-- end header -->`

 `<div id="content">`

 `<p>Charing Cross Road, London, WC2, UK</p>`

 `<p><span class="contact">Telephone</span>`

 `0207 946 0946</p>`

 `<p><span class="contact">Email</span>`

 `<a href="mailto:books@example.com">`

 `books@example.com</a></p>`

 `<iframe width="425" height="275" frameborder="0"`

 `scrolling="no" marginheight="0" marginwidth="0"`

 `src="http://maps.google.co.uk/maps?f=q&amp;`

 `source=s_q&amp;hl=en&amp;geocode=&amp;`

 `q=charing+cross+road+london&amp;output=embed">`

 `</iframe>`

 `</div><!-- end content -->`

 `<p>&copy; The Art Bookshop</p>`

`</body>`

`</html>`


3. **Chapter 17:HTML layout**

+ The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
+ The new elements provide clearer code (compared with using multiple <div> elements).
+ Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
+ To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.


4. **Chapter 18:Prossess & design**

+ It's important to understand who your target audience
is, why they would come to your site, what information
they want to find and when they are likely to return.
+ Site maps allow you to plan the structure of a site.
+ Wireframes allow you to organize the information that
will need to go on each page.
+ Design is about communication. Visual hierarchy helps
visitors understand what you are trying to tell them.
+ You can differentiate between pieces of information
using size, color, and style.
+ You can use grouping and similarity to help simplify
the information you present.


------------------------------------------------------------------------------------------------------------------------

# **JAVASCRIPT**

### **Introduction** 

- Javascripts can be used in browsers to make website more interactive by respounding to whta the user does, interesting, and user-friendly `by :`

1. **ACCESS CONTENT :**You can use JavaScript to select any
element, attribute, or text from an HTML page.
  * Select the text inside all of the <hl>elements on a page
  + Select any elements that have a class attribute with a value of note
  * Find out what was entered into a text input whose id attribute has a value of email
2. **MODIFY CONTENT:**You can use JavaScript to add
elements, attributes, and text to the page, or remove them.
  - Add a paragraph of text after the first <hl> element
  - Change the value of class attributes to trigger new CSS rules
3. **PROGRAM RULES:**You can specify a set of steps for
the browser to follow (like a recipe),which allows it to access or change the content of a page.
   -  A gallery script could check which image a user clicked on and display a larger version of that image. 



4. **REACT TO EVENTS:**You can specify that a script should run when a specific event has occurrede, it could be run when:
   - A button is pressed
   - A link is clicked (or tapped) on
   - A cursor hovers over an element 

-----------------------------------------------------------

#### **JAVASCRIPT IN THE BROWSER**
- Access the content of the page
- Modify the content of the page
- Program rules or instructions the browser can follow
- React to events triggered by the user or browser 

**```Before getting deep in the javascript this is a quiqk refresh for HTML & CSS:```**
<img src="images/read6(1).PNG" width="200" height="250"/>

---------------------------------------------------------
### **The A B C in programming**

**```Before you learn how to read and write the JavaScript
language itself, you need to become familiar with some key
concepts in computer programming and they are :```**

A. What is a script and how do I create one?
B. How do computers fit in with the world around them?
C. How do I write a script for a web page?

***A. What is a script and how do I create one?*** 
   - A script is a series of instructions that a computer can follow step by step to achieve a goal. `Sicript could be :`
       - RECIPES
       - HANDBOOKS
       - MANUALS

>A browser may use different parts of the script depending on how the user interacts with the web page.
>Script can run different sections of the code in response to the situation around them.


##### WRITING A SCRIPT
- To write a script, you need to first state your goal and then list the
tasks that need to be completed in order to achieve it. 

- Start with the big picture of what you want to achieve, and break
that down into following steps :
    1. DEFINE THE GOAL :First, you need to define the task you want to achieve. You can think of this as a puzzle for the computer to solve. 
    2. DESIGN THE SCRIPT : To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle.
    3. CODE EACH STEP : Each of the steps needs to be written in a programming language that the computer understands. In our case, this is JavaScript. 

------------------------------------------------------------

>Designing a script diagram:
<img src="images/read6(2).PNG" width="200" height="250"/>
<img src="images/read6(3).PNG" width="200" height="250"/> 

----------------------------------------------------------

##### FROM STEPS TO CODE
- Every step for every task shown in a flowchart needs to be written
in a language the computer can understand and follow.`You should focus in :`

  - You need to get to work with the:
    • Vocabulary: The words that computers understand
    • Syntax: How you put those words together to create instructions computers can follow

  - You need to learn to "think" like a computer because they solve
tasks in different ways than you or I might approach them. 

>So To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 

------------------------------------------------------------

***B. How do computers fit in with the world around them?*** 

***C. How do I write a script for a web page?***


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

- **CREATING A BASIC JAVASCRIPT** 

JavaScript is written in plain text, just like HTML and CSS,so you do not need any new tools to write a script.`And to link it with the HTML :`

1. Create a folder to put the javascript file into it `Ex; add-content . j s `
2. Use the HTML `<script>` element to tell the browser it is coming across a script. 

`<body>`

`<hl>Constructive &amp ; Co. </ hl>`

`<script src="js/ add-content.js"></ script>`

`<p>For all orders and i nquiries please cal l`

`<em>SSS-3344</ em></ p>`

`</ body>`

- **Applying objects and methods**

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

`var today= new Date();`

`var hourNow = today.getHours();`

`var greeting;`

`if (hourNow > 18) {`

`greeting= 'Good evening!';`

`else if (hourNow > 12) {`

`greeting = ' Good afternoon!';`

`else if (hourNow > 0) {`

`greeting = 'Good morni ng!';`

`else {`

`greeting = 'Welcome! ' ;`

`document .write( ' <h3>' +greeting + ' </ h3> ');` 





**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)

@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)