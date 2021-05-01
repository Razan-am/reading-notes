# **JAVASCRIPT**

### ***Chapter 3: “Object Literals”***

- WHAT IS AN OBJECT? 

  - So object is a set of variables and functions that are been grouping together to create a model of a something you would recognize from the real world. 
  - If `a variable is part of an object`, it is called a `property`. Properties tell us about the object, such as the name of a hotel or the number of rooms it has.
  - If `a function is part of an object`, it is called a `method`. Methods represent tasks that are associated with the object. 

>Example:
- This object represents a hotel. It has five properties and one method.The object is in curly braces. It is stored in a variable called hotel .

`var hotel = {`

//PROPERTIES

 These are variables

`name :  'Quay';`

`room : 40;`

`booked : 25; `

`gym : true;`

`roomTypes : ['twin' , 'double' , 'suite'];`

//METHOD

This is a function 

`checkAvailability : function (){`

 ` return this.room - this.booked ;` 
  `}`

`};`

>The example above shows how to creat an object by letiral notation (There is a several ways to creat an object)

- `To access the properties` for an object by using the `dot notation . ` and also by using the `[ ] sequar brackets`.

  - To access a property or method of an object by using the name of the object following with a period, then the name of the property or the method you want to access.

  - The `preiod is known as the member operator`. The property or the method on its right is a member of the object on its left. 

>To access the property from the example above:

`var hotelName = hotel.name;`

//or

`var hotelName = hotel ['name'] ;`

//hotel is the object

// name is the property


>To access the method from the example above:

`var roomsFree = hotel.checkAvailability ();`

>Example:

`var hotel = {`

`name: 'Park',`

`rooms: 120,`

`booked : 77,`

`checkAvailabi lity: function() {`

`return this.rooms - this.booked;`
`}`

`} ;` 

`var elName = hotel .name ;` 

`var el Rooms = hote 1 . checkAvai l abi lity();` 

-------------------------------------------------------

### ***Chapter 5: “Document Object Model”***

- The Document Object Model `(DOM)` specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

>The `DOM`  is a separate set of rules, so it is not only part in html or only in javascript.

- The `DOM` is about two areas:

**1. Making a model for an html page**

- When the loading for the webpage happened,that creat a model for that page in the memory.
- The `DOM` is an object model that made of objects , and the model called `(The DOM tree)`.And each object represents a different part of the page loaded in the browser window. 
- The `DOM` is responsible in specifies the way of how the browser should structure this model using a `DOM tree`.

**2. Accessing and changing the HTML page**

- The `DOM model` is made of objects, each object is made of methods and properties. And you can access and update eachm object in this model by the properties and methods, which in turn updates what the user sees in the browser. 
- Some people called the `DOM` an Application Programming Interface `(API)`, and it is basically let programs and scripts talk to each other. 

------------------------------------------------

**THE DOM TREE IS A MODEL OF A WEB PAGE**

 -  When the browser loads a web page, it creates a model of that page.The model is called a `DOM tree`, and it is stored in the browsers' memory. It consists of four main types of nodes:

1. `THE DOCUMENT NODE`

     Every element, attribute, and piece of text in the HTML is represented by its own `DOM node`.At the top of the tree a document node is added; it represents the entire page.

2. `ELEMENT NODES `

   The HTML elements that describe the structure of an HTML page ,like the `<hl>` lements describe what parts are headings; the `<p>` tags indicate where paragraphs of text start and finish; and so on.

>To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to. This is why you start by learning methods that allow you to access element nodes, before learning to access and alter text or attributes.

>Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file).Any changes made to the DOM tree are reflected in the browser. 

3. `ATTRIBUTE NODES`

   The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree. 

>The attribut is not the children of the element it is part of the element.

4. `TEXT NODES`

   Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node. 
   

-----------------------------------------------------

**WORKING WITH THE DOM TREE**

- Accessing and updating the DOM tree involves two steps:
   - Locate the node that represents the element you want to work with.
   - Use its text content, child elements, and attributes. 

## **Finding the elements**

### 1. ACCESS THE ELEMENTS
- It is through methods and properties that allow us to access elements

- `By selecting an individual element node :`
  1. `getElementByld()`:Uses the value of an element's id attribute
  2. `querySelector()`:Uses a CSS selector, and returns the first matching element.
  
- `By select multiple elements (nodelists) :`
  1. `getElementsByClassName()`:Selects all elements that have a specific value for their class attribute. 
  2. `getElementsByTagName()`:Selects all elements that have the
specified tag name .
  3. `querySelectorAll()`:Uses a CSS selector to select all matching elements. 

- `By traversing between elements nodes :`
  1. `parentNode`:Selects the parent of the current element node (which will return just one element). 
  2. `previousSibling / nextSibling`:Selects the previous or next
sibling from the DOM tree. 
   3. `firstChild / lastChild`:Select the first or last child of the
current element. 

### 2. WORK WITH THOSE ELEMENTS 

1. `Access/update text nodes`:The text inside any element is stored inside a text node, and to access it :
    1. Select the parent element
    2. Use the firstChild property to get the text node
    3. Use the text node's only property `(nodeValue)` to get the text from the element.

>`nodeValue`:this property lets you access or update contents of a text node. 

2. `Work with HTMl content` :
   1. `innerHTML` : allows access to child elements and text content
   2. `textContent` :Allows access just to the text content
   3. `create Element()/createTextNode()/ppendChild () / removeChild ()` :these are a several methods let you create new nodes, add nodes to a tree, and remove nodes from a tree, it is called DOM manipulation. 

3. `Access or update attribute values` :
   1. `className /id` :Lets you get or update the value of the cl ass and id attributes. 
   2. `hasAttribute()` : checks if an attribute is exists
   3. `getAttribute()` : to gets the attribute value. 
   4. `setAttri bute()` : it is to updates the attribue value. 
   5. `removeAttribute()` : it is to removes an attribute. 

----------------------------------------------

- The methods that used to find elements in the Dom tree called` Dom queries`.When you are working with an element more than once ,you should store the result for this `query in a variable`.
- It is store the location of the element(node) inside the variable 
- This save the browser from looking in tha whole DOM tree for the  element and it's known as `catching the selection`.

**ACCESSING ELEMENTS**
- DOM queries may return `one element`, or they may return a `Nodelist`, which is a collection of nodes. 

>`Nodelist:` several elements can have the same tag name, so `getElementsByTagName ()` will alwaysreturn a `Nodelist`.And if you want to select the element from this list using an `index number` (which means the numbering starts at 0 like the items in an array).

>`Fastest route:`to access an element within your web page quickly will make the page seem faster and/or more responsive.For example, `getEl ementByld ()` will quickly return one element .

**- Methods that return a single element node:**
   - `getElementByld( 'id')`:Selects an individual element given the value of its id attribute ,the HTML must have an id attribute in order for it to be selectable. 
  - `querySelector('css selector')`:Uses CSS selector syntax that would select one or more elements ,this method returns only the first of the matching elements. 

>Example:

`//By id attribute:`

`// Select the element and store it in a variable.` 

`var el = document.getElementByid('one');` 

`// Change the value of the class attribute.` 

`el.className ='cool ' ;` 

---------------------------------------------------------------------------------

**- Methods that return one or more elements `(as a Nodlist)`:**
   - `getEl ementsByClassName('class')`:Selects one or more elements given the value of their class attribute,the HTML must have a class attribute for it to be selectable.
>This method is faster than `querySelectoAll ()` . 
   - `getEl ementsByTagName('tagName')`:Selects all elements on the page with the specified tag name.
>This method is faster than `querySelectorAll ()`
   - `querySelectorAll ('css selector')`:Uses CSS selector syntax to select one or more elements and returns all of those that match.

#### ***More about the Nodlist***
-  It's a collection of element nodes,and each node is given an index number (a number that starts at zero, just like an array). 
- Nodelists look like arrays and are numbered like arrays, but they are not actually arrays; they are a type of object called a collection. 
- The order of the element nodes are stored in a Node List is the same order that they appeared in the HTML page. 
- You can select an element from the Nodlist or you can loop through each item in the Nodelist.
- Nodlist have properties and methods:
   - `The length property` tells you how many items are in the Nodelist. 
   - `The item() method` returns a specific node from the Nodelist when you tell it the index number of the item that you want.

>Example:

`var elements = document.getElementsByClassName('hot')`

`if (elements.length>= 1) {`

`var firstltem = elements.item(0);`
`}`

>You can also access it also by using the `[ ] seqaure barckets`.

>Example:

`var elements = document.getElementsByClassName('hot')`

`if (elements.length>= 1) {`

`var firstltem = elements[0];`
`} `

-------------------------------

**SELECTING ELEMENTS USING CLASS ATTRIBUTES** 

- The `getElementsByClassName()` method allows you to select elements whose class attribute contains a specific value .It is return as `a Nodlist`.
>Example:

`// Find hot items` 

`var elements = document .getEl ementsByClassName('hot');` 

`// If 3 or more are found`

`if (elements.l ength> 2) { `

`// Select the third one from the Nodelist`

`var el = elements[2];`

`// Change the value of its class attribute `

`el.className = 'cool';}`

**SELECTING ELEMENTS BY TAG NAME**

- The `get ElementsByTagName ()` method allows you to select elements using their tag name.The element name is specified as a parameter, so it is placed inside the parentheses and is contained by quote marks. 
>Example:  

`//Find <li> elements`

`var elements = document.getElementsByTagName('li ');` 

`// If 1 or more are found` 

`if (elements.length> 0) {`
 
`//Select the first one using array syntax`

`var el = elements[0];`

`//Change the value of the class attribute`

`el.className = 'cool'; }`

**SELECTING ELEMENTS USING CSS SELECTORS**
- `querySelector()` returns the first element node that matches the CSS-style selector. `querySelectorAll()`returns `a Nodelist` of all of the matches. 
>Example:

`// querySelector() only returns the first match`

`var el = document .querySel ector('li .hot ' };` 

`el.className = ' cool' ;` 

`//querySelectorAll returns a Nodelist`

`//The second matching element (the third list item) is selected and changed `

`var els = document .querySelectorAll('li .hot') ;` 

`els[1] .className = ' cool' ;` 

**LOOPING THROUGH A NODELIST**
- If you want to apply the same code to each node.
>Example:

`// Store Nodel ist i n array` 

`var hotlt ems = document .querySelectorAl l ('li.hot');`

`//If it contains item`

`if (hot ltems.length > 0) {`

`//Loop through each item`

`for (var i=0; i<hotItems.length; i++) {`

`//Change value of class attribute.`

`hotltems[i] .className = 'cool'; }`

`}`

**TRAVERSING THE DOM**
- When you have an element node, you can select another element in relation to it using these properties:
1. `parentNode:`This property finds the element
node for the containing (or parent) element in the HTML.
>`<li>element`, then its parent node would be the one representing the `<ul>element.` 
   2. `previousSibling nextSibling:`These properties find the previous or next sibling of a node if there are siblings.  
>`<li>element`, it would not have a previous sibling. However, its next sibling would be the node representing the second `<li>`
  3. `firstChild/lastChild:`These properties find the first or last child of the current element.
>`<ul> element`, the first child would be the node representing the first `<li> element`,and the lastchild would be the last `<li>`. 

```<Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.>```

- To solve this problem for the  `previousSibling nextSibling`,we use `getElementByld()`.
>Example:

`//Select the starting point and find its siblings `

`var startltem = document.getElementByid('two');`

`var prevltem startltem.previousSibling;` 

`var nextltem = startitem.nextSibling;` 

`//Change the values of the siblings' class attributes` 

`prevltem.className 'complete ' ;` 

`nextltem.className 'cool';` 

---------------------------

-To solve this problem for the  `firstChild/lastChild` we use the `getElementsByTagName()`.
>Example:

`//Select the starting point and find its children`

`var startltem = document.getElementsByTagName('ul')[0];` 

`var firstltem = startltem. firstChild;` 

`var lastltem = startitem.lastChild;` 

`//Change the values of the children's class attributes` 

`firstltem.setAttribute('class ' , 'complete');` 

`lastitem.setAttribute('class', ' cool');` 

---------------------------

## **Access/update element content**

- 



















 







   


 




 
 






 