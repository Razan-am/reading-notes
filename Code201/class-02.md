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

<img src="\\wsl$\Ubuntu\home\razan-am\reading-notes\images/1.PNG hight="350px,Width="150px">

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