# **HTML & CSS**

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
- You can include multiple CSS files in one page


**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)