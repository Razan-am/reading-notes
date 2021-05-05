# **HTML & CSS**

## ***Chapter 7: “Forms”***


- HTML forms are referring to different elements that allow you to collect information from visitors to your site.
- Forms they are like when you registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

### **Form Controls**
- The types of form controls that you can use to collect information from visitors to your site.
1. ADDING TEXT:
   - `Text input (single-line)`:used for a single line of text such
as email addresses and names.
  - `Password input`:like a single line text box but it masks `the characters entered`.
- `Text area (multi-line)`:for longer areas of text, such as messages and comments.

2. Making Choices:
  - `Radio buttons`:for use when a user must select `one of a number of options`.
  - `Checkboxes`:when a user can select and unselect `one or more options`.
  - `Drop-down boxes`:when a user must pick `one of a number of options from a list`.

3. Submitting Forms:
  - `Submit buttons`:to submit data from your form to another web page.
  -` Image buttons`:similar to submit buttons but they allow you to use an image.

4. Uploading Files:
  - `File upload`:allows users to upload files (e.g. images) to a website.

### **How Forms Work**
- A user `fills in a form` and then `presses a button to submit` the information to the server.A form may have several form controls, each gathering different information. The server needs to know `which piece of inputted data corresponds with which form element`.

### **Writing forms in HTML**
- By using the `<form> tag`,following with the `action attribute` and will usually have a `method and id attribute` too.

>`The action` :Its value is the `URL` for the page on the server that will receive the information in the form when it is submitted.

>`Method` used to sent the form using get or post methods.

>The `id` is used to identify the form distinctly from other elements on the page.

>Example:

`<form action="http://www.example.com/subscribe.php" method="get">`

`<p>This is where the form controls will appear.</p>`

`</form>`

### **Text Input**
- It is will be included inside the form tag and it's defined by using the `<input> tag` which is responsible to create several different form controls,followed with `type attribute` that will determines what kind of input they will be creating. 

>Example:

`<form action="http://www.example.com/login.php">`

`<p>Username:`

 `<input type="text" name="username" maxlength="30" />`

`</p>`

`</form>`

>`name`:It's used to tell the server which form control each piece of data was entered into. It what will be rendered to the user.

>`maxlength attribute` is used to limit the number of characters a user may enter into the text field.

### **Password Input**
- By using the `<input> tag` followed with the `type attribute` with a value of `password` it creates a text box that acts just like a `single-line text input`, except the characters are `blocked out(Hidden)`.

>Example:

`<form action="http://www.example.com/login.php">`

`<p>Username:`

 `<input type="text" name="username" maxlength="30" />`

`</p>`

`<p>Password:`
 `<input type="password" name="password" maxlength="30" />`

`</p>`

`</form>`

### **Text Area**
- By using the  `<textarea>` element and it is used to create a `mutli-line text input`.

>Example:

`<form action="http://www.example.com/comments.php">`

`<p>What did you think of this gig?</p>`

 `<textarea name="comments" cols="20" rows="4">Enter
 your comments...</textarea>`

`</form>`

>Any text that appears between the opening `<textarea>` and closing `</textarea>` tags will appear in the text box when the page loads.

### **Radio Button**
- By using the `<input> tag` followed with the `type attribute` with a value of `radio` it allow users to pick just `one of a number of options`.

>Example:

`<form action="http://www.example.com/profile.php">`

`<p>Please select your favorite genre:`

` <br />`

 `<input type="radio" name="genre" value="rock" checked="checked" />`

` Rock`

 `<input type="radio" name="genre" value="pop" />`

 `Pop`

 `<input type="radio" name="genre" value="jazz" />`

 `Jazz`

`</p>`

`</form>`

>The `value attribute` indicates the value that is sent to the server for the selected option.

>`The checked attribute` can be used to indicate which value (if any) should be selected when the page loads.Only one radio button in a group should use this attribute.

### **Checkbox**
- By using the `<input> tag` followed with the `type attribute` with a value of `checkbox` it allow users to select (and unselect) `one or more options`.

>Example:

`<form action="http://www.example.com/profile.php">`

`<p>Please select your favorite music service(s):<br />`

 `<input type="checkbox" name="service" value="itunes" checked="checked" />iTunes`

 `<input type="checkbox" name="service" value="lastfm" /> Last.fm`

 `<input type="checkbox" name="service" value="spotify" /> Spotify`

`</p>`

`</form>`


### **Drop Down List Box** 
- By using the `<select> tag` that is allows users to select one option from a drop down list. It is followed with the `name attribute` and the  `<option> element` that is specify the options that the user can select from,and the `value attribute`

>Example:

`<form action="http://www.example.com/profile.php">`

`<p>What device do you listen to music on?</p>`

`<select name="devices">`

 `<option value="ipod">iPod</option>`

 `<option value="radio">Radio</option>`

 `<option value="computer">Computer</option>`

 `</select>`

`</form>`

>In `drop down list box` if the user does not select an option, then the first item will be sent to the server as the value for this control.

### **Multiple Select Box**
- By using the `<select> tag`  followed with the `name attribute` and 
the `multiple attribute` that allow users to select `multiple options from this list`,and the `size attribute` that turn a drop down select
box into a box that shows more than one option.

>Example:

`<form action="http://www.example.com/profile.php">`

`<p>Do you play any of the following instruments?(You can select more than one option by holding down while selecting different options.)</p>`

`<select name="instruments" size="3" multiple="multiple">`

 `<option value="guitar" selected="selected">Guitar</option>`

 `<option value="drums">Drums</option>`

 `<option value="keyboard" selected="selected">Keyboard</option>`

`<option value="bass">Bass</option>`

`</select>`

`</form>`

### **File Input Box**
- By using the `<input> tag` followed with the `type attribute` with a value of `file` it allow users to upload a file.And the `type file` creates a box that looks like a text input followed by a browse button  to select a file.

>Example:

`<form action="http://www.example.com/upload.php" method="post">`

`<p>Upload your song in MP3 format:</p>`

`<input type="file" name="user-song" /><br />`

`<input type="submit" value="Upload" />`

`</form>`

### **Submit Button**
- By using the `<input> tag` followed with the `type attribute` with a value of `submit` it is used to send a form to the server.

>Example:

`<form action="http://www.example.com/subscribe.php">`

`<p>Subscribe to our email list:</p>`

`<input type="text" name="email" />`

`<input type="submit" name="subscribe" value="Subscribe" />`

`</form>`

>The value attribute is used to control the text that appears
on a button.The text will be rendered to the user.

### **Image Button**
- By using the `<input> tag` followed with the `type attribute` with a value of `image` and it's allow to use an image for the submit button.

>Example:

`<form action="http://www.example.org/subscribe.php">`

`<p>Subscribe to our email list:</p>`

 `<input type="text" name="email" />`

 `<input type="image" src="images/subscribe.jpg" width="100" height="20" />`

`</form>`

### **Button & hidden Controls**
- By using the `<button> tag` it is allow users more control over how their buttons appear and allows to combine text and images between the opening `<button> tag and closing </button> tag`.
- For the hidden control by using the `<input> tag` followed with the `type attribute` with a value of `hidden`.

>Example:

`<form action="http://www.example.com/add.php">`

`<button><img src="images/add.gif" alt="add" width="10" height="10" /> Add</button>`

`<input type="hidden" name="bookmark" value="lyrics" />`

`</form>`

```<An overall about forms>```
- Whenever you want to collect information from visitors you will need a form, which lives inside a `<form>` element.
- Information from a form is sent in name/value pairs.
- Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
- HTML5 introduces new form elements which make it
easier for visitors to fill in forms.


### **Labelling Form Controls**
- By using the `<label> tag` ,it is used to makes the form accessible to vision-impaired users,followed with the `for attribute` states which form control the label belongs to. 

>Example:

`<label>Age: <input type="text" name="age" /></label>`

`<br/ >`

`Gender:`

`<input id="female" type="radio" name="gender" value="f">`

`<label for="female">Female</label>`

`<input id="male" type="radio" name="gender" value="m">`

`<label for="male">Male</label>`

>`<label>` element is used with a checkbox or radio button.

### **Grouping Form Elements**
- By using the `<fieldset> tag`,it is allows to group related form
controls together inside the it. It is particularly helpful for `longer
forms`.
- inside it we use `<legend> element` that contains a caption which helps identify the purpose of that group of form controls.

>Example:

`<fieldset>`

`<legend>Contact details</legend>`

`<label>Email:<br />`

`<input type="text" name="email" /></label><br />`

`<label>Mobile:<br />`

`<input type="text" name="mobile" /></label><br />`

`<label>Telephone:<br />`

`<input type="text" name="telephone" /></label>`

`</fieldset>`

### **HTML5: Form Validation**
- It used when you want the form to be correctly filled and if not it will appear a message fr the user ,this is known as form validation.
And we do that by using the `required attribute` woth the value of `required`.

>Example:

`<form action="http://www.example.com/login/" method="post">`

`<label for="username">Username:</label>`

`<input type="text" name="username" required="required" /></title><br />`

`<label for="password">Password:</label>`

`<input type="password" name="password" required="required" />`

`<input type="submit" value="Submit" />`

`</form>`

### **HTML5: Date Input**
- By using the `<input> tag` followed with the `type attribute` with a value of `date` to collect a date data from the user .


>Example:

`<form action="http://www.example.com/bookings/" method="post">`

`<label for="username">Departure date:</label>`

`<input type="date" name="depart" />`

`<input type="submit" value="Submit" />`

`</form>`

### **HTML5: Email & URL Input**
1. Email:
   -  By using the `<input> tag` followed with the `type attribute` with a value of `email` to collect an email address data from the user .

>Example:

`<form action="http://www.example.org/subscribe.php">`

`<p>Please enter your email address:</p>`

`<input type="email" name="email" />`

`<input type="submit" value="Submit" />`

`</form>`

2. URL:
   - By using the `<input> tag` followed with the `type attribute` with a value of `url` to collect from a user a web page address .

>Example:

`<form action="http://www.example.org/profile.php">`

`<p>Please enter your website address:</p>`

`<input type="url" name="website" />`

`<input type="submit" value="Submit" />`

`</form>`

### **HTML5: Search Input**
- By using the `<input> tag` followed with the `type attribute` with a value of `search` to create a single line text box for search queries. It's also use the `placeholder attribute` with value is text that will be shown in the text box.

>Example:

`<form action="http://www.example.org/search.php">`

`<p>Search:</p>`

`<input type="search" name="search" placeholder="Enter keyword" />`

`<input type="submit" value="Search" />`

`</form>`

------------------------------------------------------

## ***Chapter 14: “Lists, Tables & Forms”***

- These CSS properties that were created to work with s lists, tables,
and forms.

### **Bullet Point Styles**
- It is to control the shape or style of a bullet point by using the `list-style-type property`.
   - For unordered list:
      - none, disc, circle, square.
   - For oredered list :
      - decimal,decimal-leading-zero,lower-alpha,upper-alpha,lower-roman,upper-roman.

>Example:

`ol {
list-style-type: lower-roman;} `

### **Images for Bullets**
- It is used to specify an image to act as a bullet point,by using the `list-style-image property` with the value of the url of the image.

>Example:

`ul {
list-style-image: url("images/star.png");}`

### **Positioning the Marker**
- To indicates whether the marker should appear on the inside or the outside of the box containing the main points, by using the `list-style-position` with value of:
  - `outside`:the marker sits to the left of the block of text.
  - `inside`:the marker sits inside the box of text.

>Example:

`ul.illuminations {`

`list-style-position: outside;}`

`ul.season {`

`list-style-position: inside;}`

### **List Shorthand**
- It is shorthand for the `list-style-position`,that act the same way.

>Example:

`ul {`

`list-style: inside circle;`

`width: 300px;}`

### **Table Properties**
- These properties that are commonly used with tables:
  - `width`: to set the width of the table.
  - `padding`: to set the space between the border of each table cell and its content.
   - `text-transform`: to convert the content of the table headers to uppercase.
   - `letter-spacing, font-size`: to add additional styling to the content of the table headers.
   - `border-top, border-bottom`: to set borders above and below
the table headers.
   - `text-align`: to align the writing to the left of some table cells and to the right of the others.
  - `background-color`: to change the background color of the alternating table rows.
  - `hover`: to highlight a table row when a user's mouse goes over it. 
  - `give cells padding`: for whene the text in a table cell either touches a border or another cell.

 >Example:

`table {`

`width: 600px;}`

`th, td {`

`padding: 7px 10px 10px 10px;}`

`th {`

`text-transform: uppercase;`

`letter-spacing: 0.1em;`

`font-size: 90%;`

`border-bottom: 2px solid #111111;`

`border-top: 1px solid #999;`

`text-align: left;}`

`tr.even {`

`background-color: #efefef;}`

`tr:hover {`

`background-color: #c3e6e5;}`

### **Border on Empty Cells**
- For when having an empty cells in the table we can specify whether or not their borders should be shown,by using the empty-cells property.That takes these values:
   - `show`:to shows the borders of any empty cells.
   - `hide`:to hides the borders of any empty cells.
   - `inherit`:to instructs the table cells to obey the rules of the containing table when having one table nested inside another.

>Example:

`td {`

`border: 1px solid #0088dd;`

`padding: 15px;}`

`table.one {`

`empty-cells: show;}`

`table.two {`

`empty-cells: hide;}`

### **Gaps Between Cells**
- To control the distance between adjacent cells,by using the `border-spacing property` that control the `gap`, and the `border-collapse property` that control the `collapse adjacent borders` and it's takes these values:
   - `collapse`:borders are collapsed into a single border where possible. 
   - `separate`:borders are detached from each other.

>Example:

`td {`

`background-color: #0088dd;`

`padding: 15px;`

`border: 2px solid #000000;}`

`table.one {`

`border-spacing: 5px 15px;}`

`table.two {`

`border-collapse: collapse;}`



## **```<Styling Forms>```**

### **Styling Text Inputs**
- These  properties commonly used with text inputs:
  - `font-size`: sets the size of the text entered by the user.
  - `color`: sets the text color, and `background-color` sets the background color of the input.
  - `border`: adds a border around the edge of the input box, and `border-radius` can be used to create rounded corners .
  - `focus pseudo-class` is used to change the background color of the text input when it is being used.
  - `hover psuedo-class` applies the same styles when the user hovers over them.
  - `background-image`: adds a background image to the box. 

>Example:

>`input {`

`font-size: 120%;`

`color: #5a5854;`

`background-color: #f2f2f2;`

`border: 1px solid #bdbdbd;`

`border-radius: 5px;`

`padding: 5px 5px 5px 30px;`

`background-repeat: no-repeat;`

`background-position: 8px 9px;`

`display: block;`

`margin-bottom: 10px;}`

>`input:focus {`

`background-color: #ffffff;`

`border: 1px solid #b1e1e4;}`

`input#email {`

`background-image: url("images/email.png");}`

`input#twitter {`

`background-image: url("images/twitter.png");}`

`input#web {`

`background-image: url("images/web.png");}`

### **Styling Submit Buttons**
 - These  properties commonly used with submit buttons:
   - `color`: is used to change the color of the text on the button.
   - `text-shadow`: can give a 3D look to the text .
   - `border-bottom`: has been used to make the bottom border of the button slightly thicker, which gives it a more 3D feel.
   - `background-color` can make the submit button stand out from other items around it.
   - `hover pseudo-class`: used to change the appearance of the button when the user hovers over it. 

>Example:

>`input#submit {`

`color: #444444;`

`text-shadow: 0px 1px 1px #ffffff;`

`border-bottom: 2px solid #b2b2b2;`

`background-color: #b9e4e3;`

`background: -webkit-gradient(linear, left top,`

 `left bottom, from(#beeae9), to(#a8cfce));`

`background:`

 `-moz-linear-gradient(top, #beeae9, #a8cfce);`

`background:`

 `-o-linear-gradient(top, #beeae9, #a8cfce);`

`background:`

 `-ms-linear-gradient(top, #beeae9, #a8cfce);}`

>`input#submit:hover {`

`color: #333333;`

`border: 1px solid #a4a4a4;`

`border-top: 2px solid #b2b2b2;`

`background-color: #a0dbc4;`

`background: -webkit-gradient(linear, left top,`

 `left bottom, from(#a8cfce), to(#beeae9));`

`background:`

 `-moz-linear-gradient(top, #a8cfce, #beeae9);`

`background:`

 `-o-linear-gradient(top, #a8cfce, #beeae9);`

`background:`

 `-ms-linear-gradient(top, #a8cfce, #beeae9);}`

### **Styling Fieldsets & Legends**
- `Fieldsets`: used to determining the edges of a form. In a long form they can help group together related information within it.
- `Legend` : used to indicate what information is required in the fieldset.

- These two elements include:
  - `width`: used to control the width of the fieldset. 
  - `color` :used to control the color of text.
  - `background-color` :used to change the color behind these items.
  - `border`:used to control the appearance of the border around
the fieldset and/or legend.
  - `border-radius` : used to soften the edges of these elements.
  - `padding` :used to add space inside these elements.

>Example:

`fieldset {`

`width: 350px;`

`border: 1px solid #dcdcdc;`

`border-radius: 10px;`

`padding: 20px;`

`text-align: right;}`

`legend {`

`background-color: #efefef;`

`border: 1px solid #dcdcdc;`

`border-radius: 10px;`

`padding: 10px 20px;`

`text-align: left;`

`text-transform: uppercase;}`

### **Aligning Form Controls** 
- Used to solve the alignment problem that appear by default from the row of the form. By using the `float property` to the left of the page and setting the `width property` on those elements and `text-align property` to align the titles to the right and `padding` to control the gap between the text in the title boxes and the form controls.

>Example:

`.title {`

`float: left;`

`width: 100px;`

`text-align: right;`

`padding-right: 10px;}`

`.radio-buttons label {`

`float: none;}`

`.submit {`

`text-align: right;}`

### **Cursor Styles**
- Used to control the type of mouse cursor that should be displayed
to users. By using the `cursor property`.

-The values for this property:
   - auto,crosshair,default,pointer,move,text,wait,help,url("cursor.gif").

>Example:

`a {
cursor: move;}`

----------------------------------

```<An overall about lists,tables and forms>```
-There are several elements are specifically used to control the appearance of lists, tables, and forms.
- List markers can be given different appearances using the `list-style-type` and `list-style image` properties.
- Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
- Forms are easier to use if the form controls are vertically aligned using CSS.
- Forms benefit from styles that make them feel more interactive.

------------------------------------------------------------------------------------------------------------

# **JAVASCRIPT**

## ***Chapter 6: “Events”***

Events are used to makes the page feel more interactive.


- Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
- Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
- When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
- You can use event delegation to monitor for events that happen on all of the children of an element.
- The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events. 




**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)
@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)
