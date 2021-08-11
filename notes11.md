# Chart.js
- Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.
- [Documentation for graphs](http://www.chartjs.org/docs/)

# Canvas
```
<canvas id="tutorial" width="150" height="150"></canvas>
```
- At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. 
- The `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. 
- When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.
- The `<canvas>` element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas.

## Fallback Content 
- The `<canvas>` element differs from an `<img>` tag in that, like for `<video>`, `<audio>`, or `<picture>` elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. 
- **You should always provide fallback content to be displayed by those browsers**.
- Providing fallback content is very straightforward: just insert the alternate content inside the `<canvas>` element. Browsers that don't support `<canvas>` will ignore the container and render the fallback content inside it. Browsers that do support `<canvas>` will ignore the content inside the container, and just render the canvas normally.
- The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

### Checking for support
```
var canvas = document.getElementById('tutorial');

if (canvas.getContext) {
  var ctx = canvas.getContext('2d');
  // drawing code here
} else {
  // canvas-unsupported code here
}
```

## Skeleton Template
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8"/>
    <title>Canvas tutorial</title>
    <script type="text/javascript">
      function draw() {
        var canvas = document.getElementById('tutorial');
        if (canvas.getContext) {
          var ctx = canvas.getContext('2d');
        }
      }
    </script>
    <style type="text/css">
      canvas { border: 1px solid black; }
    </style>
  </head>
  <body onload="draw();">
    <canvas id="tutorial" width="150" height="150"></canvas>
  </body>
</html>
```

## Applying styles and color
- Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
* fillStyle = color
  * Sets the style used when filling shapes.
* strokeStyle = color
  * Sets the style for shapes' outlines.
- color is a string representing a CSS <color>, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

## Transparency 
- In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha   property or by assigning a semi-transparent color to the stroke and/or fill style.
* globalAlpha = transparencyValue
  * Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

## Line styles
- There are several properties which allow us to style lines.

*lineWidth = value
  * Sets the width of lines drawn in the future.
* lineCap = type
  * Sets the appearance of the ends of lines.
* lineJoin = type
  * Sets the appearance of the "corners" where lines meet.
* miterLimit = value
  * Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
* getLineDash()
  * Returns the current line dash pattern array containing an even number of non-negative numbers.
* setLineDash(segments)
  * Sets the current line dash pattern.
* lineDashOffset = value
  * Specifies where to start a dash array on a line.
