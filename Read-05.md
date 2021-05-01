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

1. Color : it's specify the color of text inside an element, and its defined by three ways:
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

`p {
`color: rgb(100,100,90);}`

----------------------------------------------------------

2. Background-color : it's sets the color of the background for that element.

>Example:

`body {
background-color: rgb(200,200,200);}`

`h1 {
background-color: DarkCyan;}`

<img src=../imag/11.PNG width=150 hight=250>
<img src=../imag/12.PNG width=150 hight=250>

