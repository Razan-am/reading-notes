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







