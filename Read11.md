# **HTML & CSS**

## ***Chapter 16: “Images”***

- For controlling the appearance of images using CSS.
### **Controlling the size of images**
- By using the width and height properties.

 >Example:

`img.large {`

`width: 500px;`

`height: 500px;}`

### **Aligning images**
- By using the float property.

>Example:

`img.align-left {`

`float: left;`

`margin-right: 10px;}`

### **Centering images**
- Images are `inline elements` and to center an image, it should be turned into a `blocklevel element` using the `display property` with a value of `block`. Then using the the `margin property` and set the values of the `left and right margins to auto`.

>Example:

`img.align-center {`

`display: block;`

`margin: 0px auto;} `

### **Background Images**
- By using the `background-image` property and it's allows you to place an image behind any HTML element.

>Example:

`body {`

`background-image: url("images/pattern.gif");}`

### **Repeating Images**
- By using the `background-repeat` property,and it's take these values:
   - `repeat`:the background image is repeated both horizontally and vertically.
   - `repeat-x`:the image is repeated horizontally only.
   - `repeat-y`:the image is repeated vertically only.
   - `no-repeat`:the image is only shown once.

>Example:

`body {`
`background-image: url("images/tulip.gif");`
`background-repeat: no-repeat;}`

### **Fixed or not fixed images**
- By using the `background-attachment` property which specifies whether a background image should `stay in one position` or `move as the user scrolls up and down` the page. It can have one of two values:
  - `fixed`:the background image stays in the same position on the page.
  - `scroll`:the background image moves up and down as the user scrolls up and down the page.

>Example:

`body {`

`background-image: url("images/tulip.gif");`

`background-attachment: fixed;}`

### **Background Position**
- By using the `background-position` property to specify where in the browser window the background image should be placed. 
>It's takes a pair of values,the first represents the horizontal position and the second represents the vertical.

>Example:

`body {`

`background-image: url("images/tulip.gif");`

`background-repeat: no-repeat;`

`background-position: 50% 50%;}`

### **shorthand**
- By using the `background property` that acts like a shorthand for all of the other previous background properties.

>Example:

`body {`

`background: #ffffff url("images/tulip.gif")`

`no-repeat top right;}`

### **Image Rollovers & Sprites**
- It is used to create a link or button that changes to a second style when a user moves their mouse over it known as a rollover and a third style when they click on it.

>Example:

`a.button {` 

`height: 36px;`

`background-image: url("images/button-sprite.jpg");`

`text-indent: -9999px;`

`display: inline-block;}`

`a#add-to-basket {`

`width: 174px;`

`background-position: 0px 0px;}`

`a#framing-options {`

`width: 210px;`

`background-position: -175px 0px;}`

`a#add-to-basket:hover {`

`background-position: 0px -40px;}`

`a#framing-options:hover {`

`background-position: -175px -40px;}`

`a#add-to-basket:active {`

`background-position: 0px -80px;}`

`a#framing-options:active {`

`background-position: -175px -80px;}`

### **Contrast of background images**
- It's used when you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.Using the `opacity property`.

```<An over all about the images in CSS>```
- You can specify the dimensions of images using CSS,this is very helpful when you use the same sized images on several pages of your site.
- Images can be aligned both horizontally and vertically using CSS.
- You can use a background image behind the box created by any element on a page.
- Background images can appear just once or be repeated across the background of the box.
- You can create image rollover effects by moving the background position of an image.
- To reduce the number of images your browser has to load, you can create image sprites.

-----------------------------------------------------

## ***Chapter 19: “Practical Information”***

- These are a practical information that will help you launch a successful site.

### **Search Engine Optimization (SEO)**
- SEO work is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics
that your website covers.
- SEO is often split into two areas:
  1. `on-page techniques`:they are a methods you can use on your web pages to improve their rating in search engines. 
   2. `off-page techniques`:It is getting other sites to link to your website.

### **On-Page SEO**
- These are the main seven key places in the website:
  1. `Page Title`:the page title appears at the top of the browser window or on the tab of a browser.
  2. `URL / Web Address`:the name of the file is part of the URL.
  3. `Headings`:if the keywords are in a `heading <hn>` then a search engine will know that this page is all about that subject and give it  greater weight than other text.
  4. `Text`:where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. 
  5. ` Link Text`:use keywords in the text that create links between pages.
  6. `: Image Alt Text`:providing accurate descriptions of images in the `alt text`.
  7. `Page Descriptions`:the description also lives inside the `<head> element` and is specified using a `<meta> tag`.

### **To Identify The Right Keywords and Phrases**
- **Brainstorm**:list down the words that someone might type into Google to find your site.
- **Organize**:group the keywords into separate lists for the different sections or categories of your website.
- **Research**:using the several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider.
- **Compare**:it is very unlikely that your site will appear at the top of the search results for every keyword,because of there is a lot
of competition.
- **: Refine**:you need to pick which keywords you will focus on,the ones that should always be themost relevant to each section of your site.
- **Map**:picking which keywords you will use for each page.

### **Analytics: Learning about your Visitors**
- To analyzing how people found it, what they were looking at and at what point they are leaving,by using `Google Analytics`.
   
- **How Many People Are Coming to Your Site?**
  - The overview page gives you a snapshot that it tells you how many people are coming to your site.

- **What Are Your Visitors Looking At?**
  - The content link allows you to learn more about what the visitors are looking at when they come to your site.

- **Where Are Your Visitors Coming From?**
   - The traffic sources link to learn where your visitors are coming from.

### **Domain Names & Hosting**
- Domain names it is is your web address.
- Web hosting used so that other people can see your site, you will need to upload it to `a web server`.

### **FTP & Third Party Tools**
- To transfer your code and images from your computer to your hosting company, you use something known as `File Transfer Protocol`.

```<An over all about Search Engine Optimization (SEO)>```
- Search engine optimization helps visitors find your sites when using search engines.
- Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
- To put your site on the web, you will need to obtain a domain name and web hosting.
- FTP programs allow you to transfer files from your local computer to your web server.
- Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools to save you writing them from scratch.

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)




