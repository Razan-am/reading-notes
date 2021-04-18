# **HTML & CSS**


### ***Introduction to CSS***

- CSS allows you to create rules that specify how the content of an element should appear

---------------------

- Understanding CSS:`(Thinking Inside the Box)`
    - The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element.
    - CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

>Such as :

1. BLOCK & INLINE ELEMENTS
   - Block level elements look like they start on a new line taking the full width,like:
<h1>-,<h6>, <p> and <div> elements
   - Inline elements flow within the text and do not start on a new line taking only the content width,like :
 <b>, <i>,<img>, <em> and <span>

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

   -------------------

**CSS associates style rules with HTML elements :**




**CSS properties affected of how the elements are displayed**



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



**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)