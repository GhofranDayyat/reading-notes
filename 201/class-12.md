# Charts 

A great way to get started with charts is with Chart.js

## Types of graphs: 
*  line chart
* pie chart
*  bar chart

* Stepes to creat Chart :
1. the script ``<script src='Chart.min.js'></script>``
2. Drawing **line chart** ``<canvas id="buyers" width="600" height="400"></canvas>``

 **When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.**

3. Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:
 
 ``<script>``

   ``var buyers = document.getElementById('buyers').getContext('2d');``

   ``new Chart(buyers).Line(buyerData);``

 ``</script>``

4. pass some options to the chart via the **Line method**
5. Drawing a pie chart ``<canvas id="countries" width="600" height="400"></canvas>``
6. Next, we need to get the context and to instantiate the chart:

``var countries= document.getElementById("countries").getContext("2d");``

``new Chart(countries).Pie(pieData, pieOptions);``

7. Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section:

``var pieData = [``

	{

		value: 20,

		color:"#878BB6"

	},

	{

		value : 40,

		color : "#4ACAB4"

	},

	{

		value : 10,

		color : "#FF8153"

	},

	{

		value : 30,

		color : "#FFEA88"

	}

``];``

8. Now, immediately after the pieData we’ll add our options:

``var pieOptions = {``

	segmentShowStroke : false,

	animateScale : true

``}``

9. Drawing a bar chart,First, we add the canvas element: ``<canvas id="income" width="600" height="400"></canvas>``

10. retrieve the element and create the graph: 

``var income = document.getElementById("income").getContext("2d");``

``new Chart(income).Bar(barData);``

11. finally, we add in the bar chart’s data


* The `<canvas>` element differs from an ``<img>`` tag in that, like for`` <video>``, ``<audio>``, or ``<picture``> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

* **The rendering context**
 The ``<canvas>`` element has a method called`` getContext()``, used to obtain the rendering context and its drawing functions. ``getContext()`` takes one parameter, the type of context.

``var canvas = document.getElementById('tutorial');``

``var ctx = canvas.getContext('2d');``

# Drawing shapes with canvas


* **Drawing rectangles** three functions that draw rectangles on the canvas:
1. ``fillRect(x, y, width, height)`` Draws a filled rectangle.
2. ``strokeRect(x, y, width, height)`` Draws a rectangular outline.
3. ``clearRect(x, y, width, height)`` Clears the specified rectangular area, making it fully transparent.

* **Drawing paths**
1. Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.`beginPath()`
2. Methods to set different paths for objects.`Path methods`
3. Adds a straight line to the path, going to the start of the current sub-path.`closePath()`
4. Draws the shape by stroking its outline.`stroke()`
5. Draws a solid shape by filling the path's content area.`fill()`


* **Lines** 
use the``lineTo(x, y)`` method. x and y is the coordinates of the line's end point.

* **Arcs**
To draw arcs or circles, we use the arc() or arcTo() methods.

``arc(x, y, radius, startAngle, endAngle, anticlockwise)``

``arcTo(x1, y1, x2, y2, radius)``

* **Rectangles** 
``rect(x, y, width, height)``

## Applying styles and colors 
* Sets the style used when filling shapes.

``fillStyle = color``

* Sets the style for shapes' outlines.

``strokeStyle = color``

* Transparency

``globalAlpha = transparencyValue``

* **Line styles**
Sets the width of lines drawn in the future ``lineWidth = value``
Sets the appearance of the ends of lines ``lineCap = type``
Sets the appearance of the "corners" where lines meet.``lineJoin = type``

# Drawing text
The canvas rendering context provides two methods to render text:
1. Fills a given text at the given (x,y) position. Optionally with a maximum width to draw. `fillText(text, x, y [, maxWidth])`
2. Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
``strokeText(text, x, y [, maxWidth])``

## Styling text
``font = value ``The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
``textAlign = value``Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
``textBaseline = value``Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
``direction = value`` Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

## Advanced text measurements
``measureText()``



