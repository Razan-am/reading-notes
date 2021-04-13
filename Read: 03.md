# **HTML & CSS**
Design and Build Websites

## Contents:

1. **Chapter 1 :Structure** 

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


2. **Chapter 8:Extra Markup**

- **Comments in HTML**:If you add a comment to your code it will not be visible in the user's browser, you can add the text between these characters <!-- -->.


- **ID Attribute**:It is used to uniquely identify an element
from other elements,every HTML element can carry
the id,and its value should start with a letter or an underscore (not a number or any other character) like this

`<p id="pullquote">`

>it's used so that in CSS the element with a
unique identity allows you to style it differently than any other instance of the same element on the page.

- **Class Attribute**:It is used as an a way to identify several elements as being different from the other elements.

`For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements`

using this `<p class="important">`


- **Block Elements**:Some elements will always appear to start on a new line in the browser window. These are
known as block level elements.

>Examples of block elements are <h1>, <p>, <ul>, and <li>.

`<h1>Hiroshi Sugimoto</h1>`

`<p>The dates for the ORIGIN OF ART exhibition are as       follows:</p>`

`<ul> <li>Science: 21 Nov - 20 Feb 2010/11</li> </ul>`


- **Inline Elements**:Used to appear the elements are continuing on the same line as their neighbouring elements.

>Examples of inline elements are <a>, <b>, <em>, and <img>.


- **Grouping Text & Elements In a Block <div>**:Used to
group a set of elements together in one block-level box.

>For example, you might create a <div> element to contain all of the elements for the header of your site (the logo and the navigation)

`<div id="header">`

`<img src="images/logo.gif" alt="Anish Kapoor" />`

`<ul>`

 `<li><a href="index.html">Home</a></li>`

 `<li><a href="biography.html">Biography</a></li>`

 `<li><a href="works.html">Works</a></li>`

 `<li><a href="contact.html">Contact</a></li>`

`</ul>`

`</div><!-- end of header -->`


- **Grouping Text & Elements Inline <span>**:The `<span> `element acts like an inline equivalent of the `<div>` element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text
2. Contain a number of inline
elements
>The most common reason whypeople use <span> elements is so that they can control the appearance of the content of these elements using CSS.

 `<span class="gallery">Tate Modern</span>` 

 - **IFrames <iframe>**: An iframe is like a little window
that has been cut into your page — and in that window you
can see another page. The term iframe is an abbreviation of inline frame.

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

**Information About Your Pages**

**<meta>**
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




**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)