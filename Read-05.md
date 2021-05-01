# **CSS**

### ***Chapter 5: “Images”***

- Adding images in the project may be for many different reasons , it would be for `a logo, photograph, illustration, diagram, or chart.`

**1. Choosing Images for Your Site**
 - Using a great images help make the difference between an
average-looking site and a really engaging one.

>when you are building a site from scratch, the best practice is to  put all of the images the site uses inside a folder .

**2. Adding Images**
 - To add an image into the page using an` <img> tag`, It must carry be following with these two attributes:

   -` src :` it is the URL for the image.

   -` alt :` it is a text description of the image which describes the
image if it is not appearing in the web page.

**3. Changing the sizeof Images**
  - To change the height and the width of the image we use the height and width elements.

>example:

`<img src="images/quokka.jpg" alt="A family of quokka" width="600" height="450" />`

**4. Where to Place Images in Your Code**
  - The code is effect depend on where is the image is plcaed, it could be:
    1. before a paragraph
    2. inside the start of a paragraph
    3. in the middle of a paragraph

>Example:

`1. <img src="images/bird.gif" alt="Bird" width="100"
 height="100" />`

`<p>There are around 10,000 living species of birds that inhabit different ecosystems from the Arctic to the Antarctic. Many species undertake long distance annual migrations, and many more perform shorter irregular journeys.</p>`

`2. <hr />`

`<p><img src="images/bird.gif" alt="Bird" width="100" height="100" />`
`There are around 10,000 living species of birds that inhabit different ecosystems from the Arctic to the Antarctic. Many species undertake long distance annual migrations, and many more perform shorter irregular journeys.</p>`
`<hr />`

`3. <p>There are around 10,000 living species of birds that inhabit different ecosystems from the Arctic to the Antarctic.<img src="images/bird.gif" alt="Bird" width="100" height="100" />`
`Many species undertake long distance annual migrations, and many more perform shorter irregular journeys.</p>`

----------------------------------------------

```<There is three rules for creating images>```
  1. Save images in the right format (jpeg, gif, or png).
  2. Save images at the right size .
  3. Use the correct resolution.

**5. Tools to Edit & Save Images**
  - These several tools they are used to edit and save images to ensure that they are the right size, format, and resolution.Such as Adobe photoshop,Adobe illustrator. 

***- About Images***
  - The images you use on your website should be saved at the same `width and height` that you want them to appear on the page.
  - When cropping images it is important not to lose valuable information. 
  - Images created for the web should be saved at a resolution of `72 ppi`. The higher the resolution of the image, the larger the size of the file.
  - Vector images differ from bitmap images and are resolution-independent.
  - Animated `GIFs` show several frames of animage in sequence and therefore can be used to create simple animations.
  - For image that is partially transparent (or "see-through") ,the web involves selecting one of two formats:`Transparent GIF,PNG.`

**6. Figure and Figure Caption**
  - To add a caption for the images, you need to use the `<figure>` and the `<figcaption>` elements .
   - `<figure>` element it is to contain images and their caption
   - `<figcaption>` element it is used in order to allow web page authors to add a caption to an image.

>You can have more than one image inside the `<figure>` element as long as they all share the same caption.

>Example:

`<figure>`

`<img src="images/otters.jpg" alt="Photograph of two sea otters floating in water">`

`<br />`

`<figcaption>Sea otters hold hands when they sleep so they don't drift away from each other.</figcaption>`

`</figure>`

```<An overall about images>```
- The `<img>` element is used to add images to a web page.
- You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
- You should save images at the size you will be using them on the web page and in the appropriate format.
- Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

-------------------------------------------------------

### ***Chapter 11: “Color”***

- Using colors in your project it's really bring a life to it . 

**Adding the colors in CSS**

- Using colors in your project it's really bring a life to it. 

**1. Color :** it's specify the color of text inside an element, and its defined by three ways:
   - rgb values
   - hex codes
   - color names

>Example:

`/* color name */`

`h1 {`

`color: DarkCyan;}`

`/* hex code */`

`h2 {`

`color: #ee3e80;}`

`/* rgb value */`

`p {`
`color: rgb(100,100,90);}`



**2. Background-color :** it's sets the color of the background for that element.

>Example:

`body {
background-color: rgb(200,200,200);}`

`h1 {
background-color: DarkCyan;}`

--------------------------------------------------------------

```<Understanding Color>```
  - Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

  ----------------------------------------------------

>`RGB Values:`Values for `red, green, and blue` are expressed as numbers between `0 and 255.` 

>`Hex Codes:`Hex values represent values for `red, green, and blue` in `hexadecimal code.`

>`Color Names:`Colors are represented by `predefined names.`However, they are very limited in number.

>`Contrast:`When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

**3.Color  Opacity**
  - It's allows you to specify the opacity of an element and any of its child elements.The value is a number between `0.0 and 1.0` (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).Using :
  - opacity
  - rgba

>Example:

`p.one {`

`background-color: rgb(0,0,0);`

`opacity: 0.5;}`

`p.two {`

`background-color: rgb(0,0,0);`

`background-color: rgba(0,0,0,0.5);}`

**4. HSL Colors**
  - It is a y new and intuitive way to specify colors using hue, saturation, and lightness values.

`1. Hue:`it is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from `0 to 360`.

`2. Saturation:`it is the amount of gray in a color. Saturation is represented as a percentage.`100% is full saturation and 0% is a shade of gray.`

`3. Lightness:`it is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage.`0% lightness is black, 100% lightness is white, and 50% lightness is normal.`Lightness is sometimes referred to as luminosity.

-----------------------------------------------------

`- Using HSL & HSLA:`The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

  `- hue :`this is expressed as an angle (between 0 and 360 degrees).

  `- saturation :`this is expressed as a percentage.

  `- lightness :`this is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.

>Example:

`body {`

`background-color: #C8C8C8;`

`background-color: hsl(0,0%,78%);}`

`p {`

`background-color: #ffffff;`

`background-color: hsla(0,100%,100%,0.5);}`

```<An overall about colors>```
- Color not only brings your site to life, but also helps convey the mood and evokes reactions.
- There are three ways to specify colors in CSS:`RGB values, hex codes, and color names.`
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
- CSS3 has introduced an extra value for `RGB colors` to indicate opacity. It is known as`RGBA.`
- CSS3 also allows you to specify colors as `HSL values`, with an optional opacity value. It is known as `HSLA`.

--------------------------------------------------------

### ***Chapter 12: “Text”***

- Typeface Terminology
  1. Serif:Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
  2. Sans-Serif:Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
  3. Monospace:Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

## - Font wiegth:
  - The font weight not only adds emphasis but can also affect the amount of white space and contrast on a page.
  - `Wiegth (Light,Medium,Bold,Black).`

>Example:

`.credits {`

`font-weight: bold;}`

------------------------------------------------------

## - Font style:
  - Italic fonts have a cursive aspect to some of the lettering. Oblique
font styles take the normal style and put it on an angle.
   - `Style (Normal,Italic,Oblique)`

>Example:

`.credits {`

`font-style: italic;}`

-------------------------------------------------------------------

## - Font stretch:
  - In condensed versions of the font, letters are thinner and closer together. In expanded versions they are thicker and further apart. 
  - `Stretch (Condensed,Regular,Extended)`

  --------------------------------------------

### **For specifying the typeface for your webpage by using the `Font-family`**

>Example:

`body {`

 `font-family: Georgia, Times, serif;}`

 `h1, h2 {`

 `font-family: Arial, Verdana, sans-serif;}`

 `.credits {`

 `font-family: "Courier New", Courier,monospace;}`

 -------------------------------------------------------------

### **For adjust the size of the type by using the `font-size`**
  - `Units of Type Size: Pixels, Percentages, Ems.`

>Example:

`body {`

`font-family: Arial, Verdana, sans-serif;`

`font-size: 12px;}`

`h1 {`

`font-size: 200%;}`

`h2 {`

`font-size: 1.3em;}`

--------------------------------------------------

### **For using a font even if it is not installed on the computer of the person browsing,by using the `@font-face`**

>Example:

`@font-face {`

`font-family: 'ChunkFiveRegular';`

`src: url('fonts/chunkfive.eot');}`

`h1, h2 {`

`font-family: ChunkFiveRegular, Georgia, serif;}`

-----------------------------------------------------

### **For changing the case of text to uppercase or lowercase orcapitalize, by using the `text-transform`**

>Example:

`h1 {`

`text-transform: uppercase;}`

`h2 {`

`text-transform: lowercase;}`

`.credits {`

`text-transform: capitalize;}`

----------------------------------------------------

### **To control the appearance of the font, bu using the `text-decoration`**
- It is specify by the following values:
   -  `none:` this removes any decoration already applied to the text.
   - `underline:` this adds a line underneath the text.
   - `overline:` this adds a line over the top of the text.
   - `line-through:` this adds a line through words.
   - `blink:` this animates the text to make it flash on and off

>Example:

`.credits {`

`text-decoration: underline;}`

`a {`

`text-decoration: none;}`

--------------------------------------------------------

### **To adjust the text hiegth, by using the `line-height`**

>Example:

`p {`

`line-height: 1.4em;}`

------------------------------------------

### **To control the space between each letter with using the `letter-spacing` and to control the gap between words using the `word-spacing` .**

>Example:

`h1, h2 {`

`text-transform: uppercase;`

`letter-spacing: 0.2em;}`

`.credits {`

`font-weight: bold;`

`word-spacing: 1em;}`

--------------------------------------------------

### **To control the alignment of text,with using the `text-align`**
- It is n take one of four values:
  - `left:` this indicates that the text should be left-aligned.
  - `right:` this indicates that the text should be right-aligned.
  - `center:` this allows you to center text.
  - `justify:` this indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.

>Example:

`h1 {`

`text-align: left;}`

`p {`

`text-align: justify;}`

`.credits {`

`text-align: right;}`

-------------------------------------------------

### **For the vertical alignment , with use `vertical-align`**
- The values it can take are:
  - baseline
  - sub
  - super
  - top
  - text-top
  - middle
  - bottom
  - text-bottom

>Example:

`#six-months {`

`vertical-align: text-top;}`

`#one-year {`

`vertical-align: baseline;}`

`#two-years {`

`vertical-align: text-bottom;}`

---------------------------------------------------------

>It is more commonly used with inline elements such as `<img ,<em>, or <strong>` elements. And used with table cells (the `<td> and <th>` elements).

### **To indent the first line of text within an element, with using the `text-indent`.It's be specified in a number of ways but is usually given in pixels or `ems`.**

>Example:

`h1 {`

`background-image: url("images/logo.gif");`

`background-repeat: no-repeat;`

`text-indent: -9999px;}`

`.credits {`

`text-indent: 20px;}`

----------------------------------------------

### **To  create a drop shadow for a text , with using the `text-shadow`**

>Example:

`p.one {`

`background-color: #eeeeee;`

`color: #666666;`

`text-shadow: 1px 1px 0px #000000;}`

`p.two {`

`background-color: #dddddd;`

`color: #666666;`

`text-shadow: 1px 1px 3px #666666;}`

### **To specify different values for the first letter or first line of text inside an element using `first-letter` and `first-line`.**

>Example:

`p.intro:first-letter {`

`font-size: 200%;}`

`p.intro:first-line {`

`font-weight: bold;}`

------------------------------------------------

### **To change the color of links that have been visited, by using `link`, `visited`**
  - `link:` this allows you to set styles for links that have not yet been
visited.
 - `visited:` this allows you to set styles for links that have been clicked on.

>Eaxmple:

`a:link {`

`color: deeppink;`

`text-decoration: none;}`

`a:visited {`

`color: black;}`

`a:hover {`

`color: deeppink;`

`text-decoration: underline;}`

`a:active {`

`color: darkcyan;}`

---------------------------------------------

### **To change the appearance of elements when a user is interacting with them,by using `hover`, `active`, `focus`**
- `hover:` this is applied when a user hovers over an element with a pointing device such as a mouse.
- `active`: this is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked.
- `focus:` this is applied when an element has focus. Any element that you can interact with.

>Example:

`input {`

`padding: 6px 12px 6px 12px;`

`border: 1px solid #665544;`

`color: #ffffff;}`

`input.submit:hover {`

`background-color: #665544;}`

`input.submit:active {`

`background-color: chocolate;}`

`input.text {`

`color: #cccccc;}`

`input.text:focus {`

`color: #665544;}`

```<An overall about text>```
- There are properties to control the choice of font, size, weight, style, and spacing.
- There is a limited choice of fonts that you can assume most people will have installed.
- If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
- You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
- You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.


**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)

