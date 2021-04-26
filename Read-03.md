# **HTML & CSS**

### ***Chapter 3: “Lists”***

- There are lots of occasions when we need to use lists. HTML provides us with three different types:
  - `Ordered lists:`The lists where each item in the list is
numbered. 
  - `Unordered lists:`Are lists that begin with a bullet point.
  - `Definition lists:`Are made up of a set of terms along with the
definitions for each of those terms.
 
**1. Ordered Lists:**
   - The ordered lists are created by using the `<ol>` element,following with the `<li>` tag to placed the iteams inside the list.

>Example:

`<ol>`

`<li>`Chop potatoes into quarters`</li>`

`<li>`Simmer in salted water for 15-20 minutes until tender`</li>`

`</ol>`


**2. Unordered Lists:**
  - The unordered list is created by using the `<ul>` element,and it's also followed with the `<li>` tag to placed the iteams inside the list.

>Example:

`<ul>`

`<li>`1kg King Edward potatoes`</li>`

`<li>`100ml milk`</li>`

`<li>`50g salted butter`</li>`

`</ul>`

**3. Definition Lists:**
  - The definition list is created with the `<dl> `element and usually consists of a series of terms and their definitions.This type of lists are used the `<dt>` tag to contain the definition term,and also used the `<dd>` tag to contain the definition.

>Example:

`<dl>`

`<dt>`Sashimi`</dt>`

`<dd>`Sliced raw fish that is served with condiments such as shredded daikon radish or ginger root, wasabi and soy sauce`</dd>`

`<dt>`Scale`</dt>`

`<dd>`A device used to accurately measure the weight of ingredients`</dd>`

`<dd>`A technique by which the scales are removed from the skin of a fish`</dd>`

`</dl>`

***- There is another type called Nested Lists and it is used when you  put a second list inside an `<li>` element to create a sublist or nested list.***

>Examples:

`<ul>`

`<li>`Mousses`</li>`

`<li>`Pastries

 `<ul>`

 `<li>`Croissant`</li>`

 `<li>`Mille-feuille`</li>`

 `<li>`Palmier`</li>`

 `<li>`Profiterole`</li>`

 `</ul>`

`</li>`

`<li>`Tarts`</li>`

`</ul>`

```<- So an overall about the lists:>```
- There are three types of HTML lists: ordered, unordered, and definition.
-  Ordered lists use numbers.
-  Unordered lists use bullets.
- Definition lists are used to define terminology.
- Lists can be nested inside one another.

----------------------------------------------------

### ***Chapter 13: “Boxes”***

- The CSS treats each HTML element as if it lives in its own box.And there is a several properties that can be set to affect the appearance of these boxes.Such as 
  -  Control the dimensions of your boxes
  - Create borders around boxes
  - Set margins and padding for boxes
  - Show and hide boxes

**1. Control the dimensions of your boxes with (width, height):**
  - By defult the boxes are adjust into the size that just big enough to hold its contents into it,and to change it you need to use the width and hight proparities.

>Example:

`box {`

`height: 300px;`

`width: 300px;} `

- There also another option to adjust the size of the box using the `Limiting Width` by (min-width, max-width).The min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates
the maximum width a box can stretch to when the browser window is wide.

>Example:

`td.description {`

`min-width: 450px;`

`max-width: 650px;}`


- And for the `limiting hights` you will use the (min-height, max-height).

>Example:

`p {`

`min-height: 10px;`

`max-height: 30px;} `

- Overflowing Content:
  - We use it when the content contained within a box is larger than the box itself, so it help to not have a messy content.By using the (overflow) element, which we choose with it either: 
   - (hidden) to hides any extra content that does not fit in the box.
   - (scroll) that adds a scrollbar to the box so that users can scroll to see the missing content.

**2. Border, Margin & Padding:**
  - Before we get more deep in these proparities we need to differentiate between them.


**Border**

`-  border-width:`is used to control the width of a border.

>You can only use pixels or using one of the following values: thin
medium thick,to give the value fot the width.

>Example:

`p.one {`

`border-width: 2px;}`

`p.two {`

`border-width: thick;}`

`p.three {`

`border-width: 1px 4px 12px 4px;}`

`- border-style:` control the style of a border, such as solid,dotted,dashed,double,groove,ridge,inset,outset,and hidden / none for no border is shown.

>Example:

`p.one {border-style: solid;}`

`p.two {border-style: dotted;}`

`p.three {border-style: dashed;}`

`p.four {border-style: double;}`

`- border-color:`specify the color of a border using either RGB values, hex codes or CSS color names.

>Example:

`p.one {`

`border-color: #0088dd;}`

`p.two {`

`border-color: #bbbbaa #111111 #ee3e80 #0088dd;}`

>You can o individually control the colors of the borders on different sides of a box.

`- shorthand-border:`to specify the width, style and color of a border in one property.

>Example:

`p {`

`width: 250px;`

`border: 3px dotted #0088dd;}`

**Padding**

- The padding property allows you to specify how much space should appear between the content of an element and its border. 

>Example:

`p {`

`width: 275px;`

`border: 2px solid #0088dd;}`

`p.example {`

`padding: 10px;}`

>You can specify different values for each side of a box.

**Margin**
- It's controls the gap between boxes. 

>Example:

`p {`

`width: 200px;`

`border: 2px solid #0088dd;`

`padding: 10px;}`

`p.example {`

`margin: 20px;}`

>You can specify values for each side of a box.

---------------------------------------------------

```<Centering Content>```
  - If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.And you need to set a width for the box (otherwise it will take up the full width of the page).And for the text you need tohave a text-align property with its value set to center. 

>Example:

`body {`

`text-align: center;}`

`p {`

`width: 300px;`

`padding: 50px;`

`border: 20px solid #0088dd;}`

`p.example {`

`margin: 10px auto 10px auto;`

`text-align: left;}`

---------------------------------------------------

```<Change Inline/Block>```
  - Using the ( display )property allows you to turn an inline element into a block-level element or vice versa,by defining these values:
   - inline :a block-level element to act like an inline element.
   - block :an inline element to act like a block-level element.
   - inline-block :this causes a block-level element to flow like an inline element.
   - none :This hides an element from the page.

>Example:

`li {`

`display: inline;`

`margin-right: 10px;}`

`li.coming-soon {`

`display: none;}`

**3. Show and hide boxes:**
  - Using the visibility element,and it is takes two values:
     1. hidden :this hides the element.
     2. visible :this shows the element.

>Example:

`li {`

`visibility: hidden;}`

----------------------------------------------------

***There is another options to display the boxes using:***
  `- CSS3-Border Images:`It takes a backgroundimage and slices it into nine pieces. 
>This property requires three pieces of information:
1. The URL of the image
2. Where to slice the image
3. What to do with the straight edges; the possible values are: 
   - stretch stretches the image
   - repeat repeats the image
   -  round like repeat but if the tiles do not fit exactly, scales the tile image so they will.

>Example:

`p.two {`

`-moz-border-image: url("images/dots.gif")
11 11 11 11 round;`

`-webkit-border-image: url("images/dots.gif")
 11 11 11 11 round;`

`border-image: url("images/dots.gif")
 11 11 11 11 round;}`

>The box must also have a border width for the image to be shown.

`- CSS3- Box Shadows:`The box-shadow property allows you to add a drop shadow around a box.
  - Horizontal offset:Negative values position the shadow to the left of the box.
  - Vertical offset:Negative values position the shadow to the top of the box.
  - Blur distance:If omitted, the shadow is a solid line like a border.
  - Spread of shadow:If used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract.

>The inset keyword can also be used before these values to
create an inner-shadow.

>Example:

p {`

`-moz-box-shadow: 5px 5px 5px #777777;`

`-webkit-box-shadow: 5px 5px 5px #777777;`

`box-shadow: 5px 5px 5px #777777;} `

`- CSS3-Border-radius(rounded Corners):`

>You can specify individual values for each corner of a box using:
- border-top-right-radius
- border-bottom-right-radius
- border-bottom-left-radius
- border-top-left-radius

>Example:

`p {`

`border: 5px solid #cccccc;`

`padding: 20px;`

`width: 275px;`

`text-align: center;`

`border-radius: 10px;}`

`- CSS3-Elliptical Shapes (border-radius):`For more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners.

>Example:

`p.one {`

`border-top-left-radius: 80px 50px;}`

----------------------------------------------

***An overall about boxes:***
- CSS treats each HTML element as if it has its own box.
-  You can use CSS to control the dimensions of a box.
- You can also control the borders, margin and padding for each box with CSS.
- It is possible to hide elements using the display and visibility properties.
- Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
- Legibility can be improved by controlling the width of boxes containing text and the leading.
- CSS3 has introduced the ability to create image borders and rounded borders.

`==================================================================================================================`

# **JAVASCRIPT**

### ***Chapter 2: “Basic JavaScript Instructions”***

+ **ARRAYS** :
  - An array is a special type of variable. It doesn't just store one value; it stores a list of values. 

  >Example:
  
  `var colors = new Array('white ' ,'black','custom');`
  `var el = document.getElementByid( ' colors' );
  el.innerHTML = colors.item(O); `

`+ VALUES IN ARRAYS :`Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 

   **- NUMBERING ITEMS IN AN ARRAY :** Each item in an array is automatically given a number called an index. 

>`var colors;`
`colors= ['white ' ,`
`'black ' ,`
`' custom '];`

>`INDEX VALUE`
  ` o   'white '`
  ` 1 'black'`
  `2 ' custom' `

   **- ACCESSING ITEMS IN AN ARRAY :** To retrieve the third item on the list

   `>var itemThree;`
    `itemThree = col ors [2] ;`

 **-NUMBER OF ITEMS IN AN ARRAY :** Each array has a property called length, which holds the number of items in the array. 

 >`var numColors ;`
  ` numColors =colors. length;`

>// Create the array 
var colors = ['white','black' ,'custom'];
// Update the third item in the array 
colors[2] = 'beige ' ; 
//Get the element with an id of colors 
var el = document .getElementByid(' colors') ; 
//Replace with third item from the array 
el .textContent = colors[2]; 

---------------------------------------------------

### ***Chapter 4: “Decisions and Loops”***

`- Switch statments:`

A switch statement starts with a variable called the switch value.variable called the switch value.Each case indicates a possible value for this variable and the code that should run if the
variable matches that value.

>`switch (level) {`

`case 'One ':`

`title= 'Level 1 ' ;`

`break;`

`case 'Two':`

`title = ' Level 2 ' ;`

`break;`

`case ' Three' :`

`title = 'Level 3' ;`

`break ;`

`default :`

`title= 'Test';`

`break; `

`}`

>You have a default option that is run if none of the cases match.

> If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing
better performance than multiple if statements).


==========================================================================================

**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)


@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)