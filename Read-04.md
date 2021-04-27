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

