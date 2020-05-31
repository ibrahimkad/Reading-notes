# Charts

_Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create._

_A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy._




# Canvas API


**HTML Canvas Graphics**

_The HTML (canvas) element is used to draw graphics on a web page._
_The canvas> element is only a container for graphics. You must use JavaScript to actually draw the graphics._
_Canvas has several methods for drawing paths, boxes, circles, text, and adding images._

**paths**
_ A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed_


**Drawing text**
_example_


"function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}"