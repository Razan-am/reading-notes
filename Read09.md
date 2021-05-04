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
- By using the `<button> tag` it is allow users more control over how their buttons appear and allows to combine text and images
between the opening `<button> tag and closing </button> tag`.
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


**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)