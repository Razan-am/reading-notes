# **HTML & CSS**

### ***Chapter 2: “Text”***

- In creating a web page we need to use the tags that known as amarkup to the contents of the page ,these s provide extra meaning and allow browsers to show users the appropriate structure for the page.

**There is two types of markup :**
1. `Structural markup:` the elements that you can use to describe both headings and paragraphs.

2. `Semantic markup:` which provides extra information;such as quotining something.

--------------------------------------------------------------------------

**1. Structural markup:**

- `Headings`:HTML has six "levels" of headings from the `<h1>` to `<h6>`
and the diffrenation between them is about the importance and the size.

>Example:
`<h1>This is a Main Heading</h1>`

`<h2>This is a Level 2 Heading</h2>`

`<h3>This is a Level 3 Heading</h3>`

`<h4>This is a Level 4 Heading</h4>`

`<h5>This is a Level 5 Heading</h5>`

`<h6>This is a Level 6 Heading</h6>`

- `Paragraphs`:To create a paragraph, you need to include the words inside a `<p>` tag an opening`<p>`and closed one `</p>`.

>Example:
`<p>`Text is easier to understand when it is split up into units of text. For example, a book may have chapters. Chapters can have subheadings. Under each heading there will be one or more paragraphs.`</p>`

- `Bold & Italic`:To presented a words in bold style using an HTML tag, by include it insaide `<b>` tag.

>Example:
`<p>`Inside a product description you might see some `<b>`key features`</b>` in bold.`</p>`

   -For the italic style you need to include it inside `<i>` tag.

>Example:
`<p>`Captain Cook sailed to Australia on the `<i>`Endeavour`</i>`.`</p>`

- Superscript & Subscrip:It is used to make a characters that should be superscript using `<sup>` tag , or the one that should be  should be subscript using `<sub>` tag.

>Example:
`<p>`On the 4`<sup>`th`</sup>` of September you will learn about E=MC`<sup>`2`</sup>`.`</p>`
`<p>`The amount of CO`<sub>`2`</sub>` in the atmosphere grew by 2ppm in 2009`<sub>`1`</sub>`.`</p>`

- White Space:Browser usually displays the two or more spaces next to each other as one space.And if it comes across a line break, it treats that as a single space too and it's known as white space collapsing.

- `Line Breaks & Horizontal Rules`:If you wanted to add a line break inside the middle of a paragraph you can use the line break tag`<br/>` tag.

>Example:
`<p>`The Earth`<br/>`gets one hundred tons heavier every day`<br/>`due to falling space dust.`</p`>

- And for creating a break between themes you can add a horizontal rule between sections using the`<hr/>` tag, and it will be display as aline between them.

>Example:
`<p>`Venus is the only planet that rotates clockwise.`</p>`

`<hr/>`

`<p>`Jupiter is bigger than all the other planets combined.`</p>`

- Visual Editors & Their Code views:Content management systems and HTML editors usually have two views of the page you are creating: a visual editor and a code view.
  - Visual editors often resemble word processors.
  - Code views show you the code created by the visual editor so you can manually edit it ,or adding a new one.

-------------------------------------------------------------------------------------

**2. Semantic markup:**

```<It is abou the elements that don't affect the structure of your web pages, but they do add extra information to the pages .>```

- `Strong & Emphasis:`
   - `<strong> :`The strong element used for indicates that its content has strong importance.And it'll be dispaly in Bold style.
   - `<em> :`The emphasis element used for indicates emphasis that subtly changes the meaning of a sentence.And it'll display in italic style.

>Examples:
- `<p>``<strong>`Beware:`</strong>` Pickpockets operate this area.`</p>`

- `<p>`I` <em>`think`</em>` Ivy was the first.`</p>`

- `Quotations:`There are two elements commonly used for marking up
quotations:
    - `<blockquote> :`It is used for longer quotes that take up an entire paragraph.
    - `<q> :`It is used for shorter quotes that sit within a paragraph.

>Examples:
- `<blockquote cite="http://en.wikipedia.org/wiki/Winnie-the-Pooh">`

 `<p>`Did you ever stop to think, and forget to start again?`</p>`

`</blockquote>`

--------------------------------------------------------------------------------

- `<p>`As A.A. Milne said,`<q>`Some people talk to animals. Not many listen though. That's the problem.`</q>``</p>`

- `Abbreviations & Acronyms:`A title attributes on the opening tag is used to specify the full term.

>Examples: 
- `<p>``<abbr title="Professor">Prof</abbr>` Stephen  Hawking is a theoretical physicist and cosmologist.`</p>`

------------------------------------------------------------------------------

- `<p>``<acronym title="National Aeronautics and Space Administration">`NASA`</acronym>` do some crazy space stuff.`</p>`

- `Citations & Definitions:`
     - `<cite>` element can be used to indicate where the citation is from,for like referencing a piece of work such as a book.
     - `<dfn>` element can used to explain some new terminology for the first time.

>Examples:
- `<p>``<cite>`A Brief History of Time`</cite>` by Stephen Hawking has sold over ten million copies worldwide.`</p>`

----------------------------------------------------------------------------------

- `<p>`A `<dfn>`black hole`</dfn>` is a region of space from which nothing, not even light, can escape.`</p>`

- `Author Details :`Using the `<address>` element has quite a specific use it's to contain contact details for the author of the page.

>Example:
`<address>`

`<p>``<a href="mailto:homer@example.org">`

 homer@example.org`</a>``</p>`

`<p>`742 Evergreen Terrace, Springfield.`</p>`

`</address>`

- `Changes to Content :`It is used to elemets the `<del>` element can show text that has been deleted from it , and the `<ins>` element can be usedm to show content that has been inserted into a document.

>Examples:
- `<p>`It was the `<del>`worst`</del>` `<ins>`best`</ins>` idea she had ever had.`</p>`

-------------------------------------------------------------------------------------------

- `<p>`Laptop computer:`</p>`

`<p>``<s>`Was $995`</s>``</p>`

`<p>`Now only $375`</p>`

```<So the HTML elements are used to describe the structure of
the page (e.g. headings, subheadings, paragraphs).And they also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).>```

***- A full example to shown a demonstrates text markup:***

`<html>`

`<head>`

 `<title>Text</title>`

`</head>`

`<body>`

 `<h1>The Story in the Book</h1>`

 `<h2>`Chapter 1`</h2>`

 `<p>`Molly had been staring out of her window for aboutm an hour now. On her desk, lying between the copies of `<i>`Nature`</i>`, `<i>`New Scientist`</i>`, and all the other scientific journals her work had appeared in, was a well thumbed copy of `<cite>`On The Road`</cite>`. It had been Molly's favorite book since college, and the longer she spent in these four walls the more she felt she needed to be free.`</p>`

 `<p>`She had spent the last ten years in this room,sitting under a poster with an Oscar Wilde quote proclaiming that `<q>`Work is the refuge of people who have nothing better to do`</q>`. Although many considered her pioneering work, unraveling the secrets of the llama `<abbr title="Deoxyribonucleic acid">`DNA`</abbr>`, to be an outstanding achievement, Molly `<em>`did`</em>` think she had something better to do.`</p>`

`</body>`

`</html>`

-------------------------------------------------------------------------------------------

### ***Chapter 10:“Introducing CSS” ***

- CSS allows you to create rules that specify how the content of an element should appear

---------------------

- Understanding CSS:`(Thinking Inside the Box)`
    - The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.
    - CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

>Such as :

1. BLOCK & INLINE ELEMENTS
   - Block level elements look like they start on a new line taking the full width,like:
`<h1>-,<h6>, <p> and <div> elements`
   - Inline elements flow within the text and do not start on a new line taking only the content width,like :
 `<b>, <i>,<img>, <em> and <span>`


>Example Styles:
  - Boxes:
  - Width and height
  - Borders (color, width, and style)
  - Background color and images
   - Position in the browser window.
- Text :
  - Typeface
  - Size
  - Color
  - Italics, bold, uppercase,
  - lowercase, small-caps
- Specific :
   - Lists
   - Tabels
   - Forms 

----------------------------------------------------------------------

**CSS associates style rules with HTML elements :**


**CSS properties affected of how the elements are displayed**



<img src="images/2.PNG" width="250" height="150" />


>Examples:
HTML file:

`<!DOCTYPE html>`

`<html>`

`<head>`

 `<title>Introducing CSS</title>`

 `<link href="css/example.css" type="text/css"`

` rel="stylesheet" />`

`</head>`

`<body>`

` <h1>From Garden to Plate</h1>`

 `<p>A`

  `<i>potager</i>` 
  `is a French term for an`
 `ornamental vegetable or kitchen garden ... </p>`

 `<h2>What to Plant</h2>`

 `<p>Plants are chosen as much for their functionality`
 `as for their color and form ... </p>`

`</body>`

`</html>`

>CSS file:
body {

>font-family: Arial, Verdana, sans-serif;
}
h1, h2 {

>color: #ee3e80;
}
p {

>color: #665544;
}

----------------------------------------------------------

### ***Ways to link CSS with HTML:***

1. Inline : by applying the style directly to the element in tag .


2. Internal CSS: include CSS rules within an HTML page by placing them inside a `<style>` element, which usually sits inside the `<head>` element of the page. 


3. External CSS : using the `<link>` element in the HTML document to tell the browser where to find the CSS file that is used to style the page. 

-----------------------------------------------------------

### ***CSS Selectors:***
- There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document. 
>Such as : (*) to target all the elements, (h1,h2,.....) by targetting the elemnt name 

----------------------------------------------------------

### ***Inheritance:***
- If you specify the font-family or color properties on the `<body>` element, they will apply to most child elements. This is because the value of the font-family property is inherited by child elements.

----------------------------------------------------------
### ***An Overall***
- CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
- Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
- Different types of selectors allow you to target your rules at different elements.
- Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document, although they may appear within an HTML page.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# **JAVASCRIPT**

### ***Chapter 2: “Basic JavaScript Instructions”***

+ **STATEMENTS** :Statement are instructionsand each one starts on a new line, and it can be organized into code blocks by surround it with curly braces ({});these are known as code blocks.

+ **COMMENTS** :You should write comments to explain what your code does.  There is two ways to write comments:
1. Using `/* */` and its for multi-line comments .
2. Using `//` and its for single-line comments.

+ **A VARIABLE** :A data that is temporarily store information it needs to do a certine job.

<img src="images/3.PNG"  hight="150px Width="250px">

<img src="images/4.PNG"  hight="150px Width="250px">

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

+ **CHANGING THE VALUE OF A VARIABLE** :
  - Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script.

+ **RULES FOR NAMING VARIABLES** :
  - The name must begin with a letter, dollar sign `($)`,or an underscore `(_)`. `It must not start with a number.` 
  - The name can contain letters,numbers, dollar sign `($)`, or an underscore `(_)`. Note that you must not use a dash`(-)` or a period `(.)` `in a variable name. `
  - You cannot use keywords or reserved words. 
  - All variables are case sensitive.
  - Use a name that describes the kind of information that the variable stores.
  - If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word.

  ---------------------------------------------------------------------

+ **ARRAYS** :
  - An array is a special type of variable. It doesn't just store one value; it stores a list of values. 

  >Example:
  var colors = new Array('white ' ,'black','custom');
  var el = document.getElementByid( ' colors' );
  el.innerHTML = colors.item(O); 

+ VALUES IN ARRAYS :Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 
   - NUMBERING ITEMS IN AN ARRAY :Each item in an array is automatically given a number called an index. 
>var col ors;
colors= ['white ' ,
'black ' ,
' custom '];
>INDEX VALUE
   o   'white '
   1 'black'
   2 ' custom' 

   - ACCESSING ITEMS IN AN ARRAY :To retrieve the third item on the list
   >var itemThr ee;
    itemThree = col ors [2] ;

    -NUMBER OF ITEMS IN AN ARRAY :Each array has a property called length, which holds the number of items in the array. 
    >var numColors ;
     numColors =colors. length; 

>// Create the array 
var colors = ['white','black' ,'custom'];
// Update the third item in the array 
colors[2] = 'beige ' ; 
//Get the element with an id of colors 
var el = document .getElementByid(' colors') ; 
//Replace with third item from the array 
el .textContent = colors[2]; 

------------------------------------------------------------------------

** EXPRESSIONS:**
  - Evaluates into (results in) a single value,there are `two types of expressions:`
    1. Expressions that just assign a value to avariable.
`var color = 'beige';` 
     2. Exepressions that use two or more values to return a single value .
     `var area = 3 * 2;` 

** OPERATORS:**
  - They allow programmers tocreate a single value from one or more values, it's devided to :
  1. Assignment operators
###### Assign a value to a variable
`color = 'beige';`
###### The value of co 1 or is now beige
  2. Arithmetic operators
###### Perform basic math
`area = 3 * 2;`
###### The value of area is now 6. 
 3. String operators
###### Combine two strings
`greeting= 'Hi 1 + 'Mol ly';`
###### The value of greeting is now Hi Molly.
  4. Comparison operators
###### Compare two values and return true or false
`buy = 3 > 5;`
###### The value of buy is false. 
   5. Logical operators 
###### Combine expressions and return true or false
`buy= (5 > 3) && (2 < 4);`
###### The value of buy is now true. 

***- Arithmetic operators :***
- JavaScript contains the following mathematical operators, which you can use with numbers.


>Example for arithmetic operator:
// Subtotal is 70 
var subtotal (13 + 1) * 5;
// Shipping is 7 
var shipping 0.5 * (13 + 1) ;
// Total is 77
var total subtotal + shipping ;

>var el Sub document .getElementByid(' subtotal ') ;
elSub .textContent =subtotal ; 

>var elShip = document .getElement Byid('shi ppi ng ') ;
elShip.textContent =shipping; 

>var elTotal = document .getElementByid('total ');
elTotal .textContent =total; 

------------------------------------------------------------

***- Srting operator :***
- There is just one string operator: the+ symbol. It is used to join the strings on either side of it.

>Example:
var greeting= 'Howdy ';
var name= 'Mol ly' ; 
var welcomeMessage = greeting+ name+ '!'; 
var el = document.getElementByld('greeting');
el .textContent = welcomeMessage;

-----------------------------------------------------------------------------

### ***Chapter 4: “Decisions and Loops”***

- Switch statments:

A switch statement starts with a variable called the switch value.variable called the switch value.Each case indicates a possible value for this variable and the code that should run if the
variable matches that value.

>switch (level) {

case 'One ':
title= 'Level 1 ' ;
break;

case 'Two':
tit 1 e = ' Level 2 ' ;
break;

case ' Three' :
title = 'Level 3' ;
break ;

default :
title= 'Test';
break; 

}

>You have a default option that is run if none of the cases match.
> If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing
better performance than multiple if statements).















**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)


@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)