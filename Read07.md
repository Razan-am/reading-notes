# **HTML & CSS**

### ***Chapter 6: “Tables”***

- Tables represents information in a grid format and they are used for several things such as:sports results, stock
reports, train timetables.

**Basic Table Structure**
- By using the `<thable>` element, with the `<tr> `which indicate indicate the start of each row,and the `<td>` which indicate the cell of a table.

>Example:

`<table>`

 `<tr>`

 `<td>15</td>`

 `<td>15</td>`

 `<td>30</td>`

` </tr>`

`</table>`

**Table Headings**
- By using the` <th>` element and its purpose is to represent the heading for either a column or a row.
>Example:

`<table>`

 `<tr>`

 `<th></th>`

 `<th scope="col">Saturday</th>`

 `<th scope="col">Sunday</th>`

 `</tr>`

 `<tr>`

 `<th scope="row">Tickets sold:</th>`

 `<td>120</td>`

 `<td>135</td>`

`</tr>`

`</table>`

**Spanning Columns**
- It is used when you need the entries in a table to stretch across more than one column. By using the `colspan attribute` and it can be
used on a `<th>` or `<td>` element.
>Example:

`<table>`

`<tr>`

 `<th>Monday</th>`

 `<td colspan="2">Geography</td>`

 `<td>Math</td>`

 `<td>Art</td>`

 `</tr>`

`</table>`

**Spanning Rows**
- It is used when you need entries in a table to stretch down across more than one row. By using the r`owspan attribute` can be used on a `<th>` or `<td>` element.
>Example:

`<table>`

`<th>6pm - 7pm</th>`

 `<td rowspan="2">Movie</td>`

 `<td>Comedy</td>`

 `<td>News</td>`

 `</tr>`

`</table>`

**Long Tables**
- `<thead>`: the headings of the table should sit inside the `<thead>` element.
- `<tbody>`: the body should sit inside the `<tbody>`element.
- `<tfoot>`: the footer belongs inside the`<tfoot>` element.

```<An over all about tabels>```
- The `<table>` element is used to add tables to a web page.
- A table is drawn out row by row. Each row is created with the `<tr>` element.
- Inside each row there are a number of cells represented by the `<td>` element or `<th>` if it is a header.
- You can make cells of a table span more than one row or column using the `rowspan` and `colspan` attributes.
- For long tables you can split the table into a `<thead>`, `<tbody>`, and `<tfoot>`.

=======================================================

# **JAVASCRIPT**

### ***Chapter 3 (first part): “Functions, Methods, and Objects”***

- ### **Function & methods**

- Complex scripts can run to hundreds (even thousands) of lines so programm function used to organize their code.
 
***- Function and method :***

`1. Functions :`consist of a series of statements that have been grouped together because they perform a specific task.

>If different parts of a script repeat the same task, you can
reuse the function.

  - **Calling the function:** you need to give your function a name , and the name should describe the task it is `performing.So` you could o ask the function to perform its task later and when you ask it to perform its task that's known as `calling the function`

   - **Code block :** the `steps/statments` that the function need to  perform in order to perform its task.

   - **Parameters :** it is the informations that are provided to the function in order to achieve a given task.

   -  **Return value :** When you write a function and you expect it to provide you with an answer, the response is known as `a return value.`


>Example:

`//variable`

`var msg = 'Sign up to receive our newsletter for 10%` `off!';`

`//function `

`function updateMessage() {`

`var el = document.getElementByld('message'};`

`el .textContent = msg;}`

`//calling the function`

`updateMessage(}; `

<img src=imag/7.PNG width=150 hight=250>
<img src=imag/8.PNG width=200 hight=350>
<img src=imag/9.PNG width=150 hight=250>
<img src=imag/10.PNG width=200 hight=350>

-------------------------------------------------------

**References:**

@Jon Duckett/[HTML & CSS
](file:///D:/ltuc/code%20102/HTML%20CSS.pdf)


@Jon Duckett/[JAVASCRIPT
](file:///D:/ltuc/code%20102/Javascript_and_jquery_interactive_jon_du.pdff)