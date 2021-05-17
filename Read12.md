# **Chart.js, Canvas**

## ***Chart***
- Charts are used to displaying data visually and it is an better way to display the data than using than tables.
- To get started with charts is with `Chart.js`, and it's a JavaScript plugin that uses `HTML5’s canvas element` to draw the graph onto the page.

**The `canvas element` in our HTML**
- It will be added to the body of our HTML page.

>Example:

`<canvas id="buyers" width="600" height="400"></canvas>`

- For creating charts you need to set a script code include in your page along with a single `<canvas>` node to render the chart.

>Example:

`<canvas id="myChart" width="400" height="400"></canvas>`

`<script>`

`var ctx = document.getElementById('myChart').getContext('2d');`

`var myChart = new Chart(ctx, {`

`type: 'bar',`

` data: {`

        `labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],`

        `datasets: [{`

           `label: '# of Votes',`

            `data: [12, 19, 3, 5, 2, 3],`

            `backgroundColor: [`

                `'rgba(255, 99, 132, 0.2)',`

                `'rgba(54, 162, 235, 0.2)',`

           ` ],`

            `borderColor: [`

                `'rgba(255, 99, 132, 1)',`

                `'rgba(54, 162, 235, 1)',`

          `  ],`

            `borderWidth: 1`

        `}]`

    `},`

    `options: {`

        `scales: {`

           `y: {`

                `beginAtZero: true`

           ` }`

        `}`

    `}`

`});`

`</script>`

>Chart.js is available under the MIT license.

>The great things about Chart.js are that it’s simple to use and really very flexible.

------------------------------------------------------

## ***Canvas API***

- Canvas is an html element:

`<canvas id="tutorial" width="150" height="150"></canvas>`

It's takes only two attributes, `width and height`,also it can added to it an `id attribute` and It is always a good idea to supply it because this makes it much easier to identify it in a script.

>Browsers that don't support `<canvas>` will ignore the container and render the fallback content inside it. Browsers that do support `<canvas>` will ignore the content inside the container, and just render the canvas normally.

### **Required  for the `</canvas>` tag**
- It's requires the closing tag `</canvas>`,if this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.

### **The rendering context**
- `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, and it has a method called `getContext()`, used to obtain the rendering context and its drawing functions.

>Example:

`var canvas = document.getElementById('tutorial');`

`var ctx = canvas.getContext('2d');`

>The first line in the script retrieves the node in the DOM representing the `<canvas>` element by calling the `document.getElementById()` method. Once you have the element node, you can access the drawing context using its `getContext()` method.

### **Drawing shapes with canvas**
- We can use the canvas to draw different shapes such as:` rectangles, triangles, lines, arcs and curves`.

 **The grid**
-  Canvas has grid or coordinate space, by default grid overlayed normally is 1 unit in the grid which corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0),and all elements are placed relative to this origin. 

>`<canvas>` only supports two primitive shapes: rectangles and paths lists of points connected by lines,but for the complex shapes there is an assortment of path drawing functions which make it possible to draw them.

**Drawing rectangles**
- There are three functions that draw rectangles on the canvas:

`fillRect(x, y, width, height)`
>Draws a filled rectangle.

`strokeRect(x, y, width, height)`

>Draws a rectangular outline.

`clearRect(x, y, width, height)`

>Clears the specified rectangular area, making it fully transparent.

>`x and y` specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle, `width and height` provide the rectangle's size.

>Example:

`function draw() {`

 `var canvas = document.getElementById('canvas');`

  `if (canvas.getContext) {`

   `var ctx = canvas.getContext('2d');`

`ctx.fillRect(25, 25, 100, 100);`

`ctx.clearRect(45, 45, 60, 60);`

   `ctx.strokeRect(50, 50, 50, 50);`

  `}`

`}`

>`fillRect()` function draws a large black square 100 pixels on each side,`clearRect()` function then erases a 60x60 pixel square from the center, and `strokeRect()` is called to create a rectangular outline 50x50 pixels within the cleared square.

**Drawing paths**
- A path is a list of points, connected by segments of lines that can be of different shapes,to draw the path we need to :
   - First, you create the path.
   - Then you use drawing commands to draw into the path.
   - Once the path has been created, you can stroke or fill the path to render it.

- Functions used to perform these steps:

`beginPath()`

>The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape.

`Path methods`

>The second step is calling the methods that actually specify the paths to be drawn..

`closePath()`

>The third, is to call closePath(). This method tries to close the shape by drawing a straight line from the current point to the start. 

`stroke()`

>Draws the shape by stroking its outline.

`fill()`

>Draws a solid shape by filling the path's content area.

**Drawing a triangle using path**
>Example:

`function draw() {`

  `var canvas = document.getElementById('canvas');`

  `if (canvas.getContext) {`

 `var ctx = canvas.getContext('2d');`

 `ctx.beginPath();`

 `ctx.moveTo(75, 50);`

 `ctx.lineTo(100, 75);`

`ctx.lineTo(100, 25);`

`ctx.fill();`

  `}`

`}`

>The `moveTo()` function is to place the starting point somewhere else,we could also use `moveTo()` to draw unconnected paths.

- `moveTo(x, y)`:
Moves the pen to the coordinates specified by x and y.

**Drawing a smily face using line**

>Example:

`function draw() {`

`var canvas = document.getElementById('canvas');`

  `if (canvas.getContext) {`

`var ctx = canvas.getContext('2d');`

 `ctx.beginPath();`

 `ctx.arc(75, 75, 50, 0, Math.PI * 2, true); // Outer circle`

 `ctx.moveTo(110, 75);`

 `ctx.arc(75, 75, 35, 0, Math.PI, false);  // Mouth (clockwise)`

`ctx.moveTo(65, 65);`

 `ctx.arc(60, 65, 5, 0, Math.PI * 2, true);  // 
    Left eye`

`ctx.moveTo(95, 65);`

`ctx.arc(90, 65, 5, 0, Math.PI * 2, true);  // Right eye`

`ctx.stroke();`

  `}`

`}`

**Lines** 
- For drawing straight lines, use the `lineTo()` method. 
 
  -`line To(x, y)` :
Draws a line from the current drawing position to the position specified by x and y.

>Example:

`function draw() {`

 `var canvas = document.getElementById('canvas');`

  `if (canvas.getContext) {`

   `var ctx = canvas.getContext('2d');`

   `// Filled triangle`

  `ctx.beginPath();`

   `ctx.moveTo(25, 25);`

  `ctx.lineTo(105, 25);`

  `ctx.lineTo(25, 105);`

  `ctx.fill();`

   `// Stroked triangle`

   `ctx.beginPath();`

  `ctx.moveTo(125, 125);`

  `ctx.lineTo(125, 45);`

 `ctx.lineTo(45, 125);`

 `ctx.closePath();`

`ctx.stroke();`

  `}`

`}`

**Drawing Arcs**
- To draw arcs or circles, we use the `arc() or arcTo()` methods.

   - `arc`(x, y, radius, startAngle, endAngle, counterclockwise):
 `x and y` are the coordinates of the center of the circle on which the arc should be drawn,radius is self-explanatory. The `startAngle and endAngle` parameters define the start and end points of the arc in radians, along the curve of the circle. These are measured from the x axis. The `counterclockwise` parameter is a Boolean value which, when `true`, draws the arc counterclockwise; otherwise, the arc is `drawn clockwise`.

  - `arcTo(x1, y1, x2, y2, radius)`:
Draws an arc with the given control points and radius, connected to the previous point by a straight line.


**References:**

@ SARA VIEIRA /[CHART.JS
](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

@Chart.js contributors/[CHART.JS
](https://www.chartjs.org/docs/latest/)

@Mozilla and individual contributors/[canvas
](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)