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

   The HTML elements that describe the structure of an HTML page ,like the `<hl>` lements describe what parts are headings; the <p> tags indicate where paragraphs of text start and finish; and so on.

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

### 1. ACCESS THE ELEMENTS
- It is through methods and properties that allow us to access elements

- By selecting an individual element node :
  1. `getElementByld()`:Uses the value of an element's id attribute
  2. `querySelector()`:Uses a CSS selector, and returns the first matching element.
  
- By select multiple elements (nodelists) :
  1. `getElementsByClassName()`:Selects all elements that have a specific value for their class attribute. 
  2. `getElementsByTagName()`:Selects all elements that have the
specified tag name .
  3. `querySelectorAll()`:Uses a CSS selector to select all matching elements. 

- By traversing between elements nodes :
  1. `parentNode`:Selects the parent of the current element node (which will return just one element). 
  2. `previousSibling / nextSibling`:Selects the previous or next
sibling from the DOM tree. 
   3. `firstChild / lastChild`:Select the first or last child of the
current element. 

### 2. WORK W ITH THOSE ELEMENTS 

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

   








 







   


 




 
 






 