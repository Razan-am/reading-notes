# **HTML & CSS**

### ***Chapter 4: Ch.4 “Links”***

- Using links allows you to move from one web page to another.

- There is several types of links :
  1. Links from one website to another.
  2. Links from one page to another on the same website.
  3. Links from one part of a web page to another part of the same page.
  4. Links that open in a new browser window.
  5. Links that start up your email program and address a new email to someone.

**-How to write a link :**
- It is created using the `<a>` element,and the users can click on anything between the opening `<a>` tag and the closing `</a>` tag.The link between them is specify which page you want to be transfer to
 using the `href attribute` inside it.

>Example:

`<a href="http://www.imdb.com">IMDB</a>`

**- Linking to Other Sites**
  - Using the `<a>` tag and the value of the `href attribute` is the page that you want people to go to when they click on the link.

>Example:

`<p>Movie Reviews:`

`<ul>`

 `<li>`

`<a href="http://www.empireonline.com">Empire</a>`

`</li>`

 `<li>`

`<a href="http://www.metacritic.com">Metacritic</a>`

`</li>`

`</ul>`

`</p>`

**- Linking to Other Pages on the Same Site**
 - Using the `<a>` tag and `a relative URL` ,if the pages of the site are in the same folder, the value of the `href attribute` is just the name of the file.If it is in differents folerds you need to mention the folder name first.

>Example:

`<p>`

`<ul>`

`<li>`

`<a href="index.html">Home</a>`

`</li>`

`<li>`

`<a href="about-us.html">About</a>`

`</li>`

`</ul>`

`</p>`

>Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

**- Email Links**
- By using the `<a>` tag and the `href` will be followed with `mailto:` and is followed by the email address you want the email to be sent to.

>Example:

`<a href="mailto:jon@example.org">Email Jon</a>`

**- Opening Links in a New Window**
- It is by using the `<a>` tag with something called target attribute on the opening `<a>` tag, which send the user to new window.

>Example:

`<a href="http://www.imdb.com" target="_blank"> `

**- Linking to a Specific Part of the Same Page**
- It is used when you want the user to reach to the sections lower down or to page back to the top of it to save users from having to scroll back to the top.
  - By using the `<a>` tag and the `id attribute` that identify those sections of the page.

>Example:

`<h1 id="top">Film-Making Terms</h1>`

`<a href="#arc_shot">Arc Shot</a><br />`

`<a href="#interlude">Interlude</a><br />`

`<h2 id="arc_shot">Arc Shot</h2>`

`<p>A shot in which the subject is photographed by an encircling or moving camera</p>`

`<h2 id="interlude">Interlude</h2>`

`<p>A brief, intervening film scene or sequence, not specifically tied to the plot, that appears within a film</p>`

**- Linking to a Specific Part of Another Page**
  - link to a specific part of a different page `(whether on your own site or a different website),` the page you want to link to must have an `id attributes` that identify specific parts of the page.
  - The `href attribute` will contain the address for the page `(either an absolute URL or a relative URL)`, followed by the `# `symbol, followed by the value of the `id attribute` that is used on the element you are linking to.

```<An overall about the links:>```
- Links are created using the `<a>` element.
- The `<a>` element uses the `href attribute` to indicate the page you are linking to.
- If you are linking to a page within your own site, it is best to use `relative links` rather than qualified URLs.
- You can create links to open email programs with an email address in the "to" field.
- You can use the `id attribute` to target elements within a page that can be linked to.

-------------------------------------------------------

### ***Chapter 15: “Layout”***

- The layout are about us know and to control where each element sits on a page and how to create attractive page layouts.

- Key Concepts in Positioning Elements:

- CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

- Block-level elements start on a new line:

>`<h1> <p> <ul> <li>`

- Inline elements flow in between surrounding text:

>`<img> <b> <i>`

`- Containing Elements:` If one block-level element sits inside another
block-level element then the outer box is known as the containing or parent element.

`- Controlling the Position of Elements:`

  `1. Normal Flow (position-static):`
   each block-level element sits on top of the next one. 

  `2. Relative Positioning (position-relative):`
     It's moves an element in relation to where it would have been in normal flow.

>Example:

`p.example {`

`position: relative;`

`top: 10px;`

`left: 100px;}`

--------------------------------------

`3. Absolute Positioning(position-absolute):`
When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.

>Example:

`h1 {`

`position: absolute;`

`top: 0px;`

`left: 500px;`

`width: 250px;}`

`3. Fixed Positioning(position-fixed):`
It is a type of absolute positioning that requires the position property to have a value of fixed.

>Example:

`h1 {`

`position: fixed;`

`top: 0px;`

`left: 50px;`

`padding: 10px;`

`margin: 0px;`

`width: 100%;`

`background-color: #efefef;}`

`4. Overlapping Elements(z-index):`
It is used to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front. 

>Example:

`h1 {`

`position: fixed;`

`width: 100%;`

`background-color: #efefef;`

`z-index: 10;}`


`5. Floating Elements(float):`
It is allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

>Example:

`blockquote {`

 `float: right;`

 `width: 275px;`

 `font-size: 130%;`

 `font-style: italic;}`

>You can use the float to place the box elements side by side.

---------------------------------------------

`6. Clearing Floats(clear):`
It's allows you to say that no element within the same containing element should touch the left or righthand sides of a box,and it is takes:

  `- left:`which means the left-hand side of the box should not touch any other elements

  `- right:`which mean the right-hand side of the box will not touch elements appearing in the same containing element.

>If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.

---------------------------------------------------

- To solve the problem that appears when adding an extra element after the last floated box inside the containing element,using this :
   - The overflow property is given a value auto.
   - The width property is set to 100%.

>Example:

`div {`

`border: 1px solid #665544;`

`overflow: auto;`

`width: 100%;}`

`- Creating Multi-Column Layouts with Floats:`
To use multiple columns in the design, it will achieved by using a`<div>` element to represent each column. And these following CSS properties to place the columns next to each other.
   - width:this sets the width of the columns.
   - float:this positions the columns next to each other
   - margin:this creates a gap between the columns.

>Example:

`.column1of2 {`

`float: left;`

`width: 620px;`

`margin: 10px;}`

`.column2of2 {`

`float: left;`

`width: 300px;`

`margin: 10px;}`


**Screen Sizes**
- There is different sized screens that show different amounts of information of the web page, so the design needs to be able to
work on a range of different sized screens.

`1. Screen Resolution:`
  - It is refers to the number of dots a screen shows per inch.

`2. Page Sizes:`
  - Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.

`3. Fixed Width Layouts:`
  - Fixed width layout designs do not change size as the user increases or decreases the size of their browser window.

>Measurements tend to be given in pixels

`4. Liquid Layouts:`
  - The liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. 

>They tend to use percentages.

---------------------------------------------------

```<An overall about the layout:>```
- <div> elements are often used as containing elements to group together sections of a page.
- Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
- Pages can be fixed width or liquid (stretchy) layouts.
- Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS Frameworks provide rules for common tasks.
- You can include multiple CSS files in one page.

================================================================================================

# **JAVASCRIPT**

### ***Chapter 3 (first part): “Functions, Methods, and Objects”***

- ### **Function & methods**

- Complex scripts can run to hundreds (even thousands) of lines so programm function used to organize their code.
 
***- Function and method :***

`1. Functions :`consist of a series of statements that have been grouped together because they perform a specific task.

>If different parts of a script repeat the same task, you can
reuse the function.

  - **Calling the function:** you need to give your function a name , and the name should describe the task it is `performing.So` you could o ask the function to perform its task later and when you ask it to perform its task that's known as `calling the function`

   - **Code block :** the `steps/statments` that the function need to  perform in order to perform its task.

   - **Parameters :** it is the informations that are provided to the function in order to achieve a given task.

   -  **Return value :** When you write a function and you expect it to provide you with an answer, the response is known as `a return value.`


>Example:

`//variable`

`var msg = 'Sign up to receive our newsletter for 10%` `off!';`

`//function `

`function updateMessage() {`

`var el = document.getElementByld('message'};`

`el .textContent = msg;}`

`//calling the function`

`updateMessage(}; `

<img src=imag/7.PNG width=150 hight=250>
<img src=imag/8.PNG width=200 hight=350>
<img src=imag/9.PNG width=150 hight=250>
<img src=imag/10.PNG width=200 hight=350>

-------------------------------------------------------

**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)


@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)

