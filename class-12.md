# Charts

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

**Setting up**

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory we’ll be working in. Then create a new html page and import the script.

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page.

Then we need to drawing a pie chart and finally drawing a bar chart.

**Canvas**

<*canvas>* looks like the <*img>* element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the <*canvas>* element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.


The <*canvas>* element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

The <*canvas>* element has a method called getContext(), used to obtain the rendering context and its drawing functions.

The script includes a function called draw(), which is executed once the page finishes loading; this is done by listening for the load event on the document.

![can](https://www.w3.org/TR/2009/WD-html5-20090825/images/drawImage.png)


There are three functions that draw rectangles on the canvas:

* fillRect(x, y, width, height)
Draws a filled rectangle.

* strokeRect(x, y, width, height)
Draws a rectangular outline.

* clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.


Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.


**Drawing paths**

* beginPath()
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.

* Path methods
Methods to set different paths for objects.

* closePath()
Adds a straight line to the path, going to the start of the current sub-path.

* stroke()
Draws the shape by stroking its outline.

* fill()
Draws a solid shape by filling the path's content area.


For drawing straight lines, use the lineTo() method.

**lineTo(x, y)**

Draws a line from the current drawing position to the position specified by x and y.

To draw arcs or circles, we use the arc() or arcTo() methods.

**arc(x, y, radius, startAngle, endAngle, anticlockwise)**

Draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending at endAngle going in the given direction indicated by anticlockwise (defaulting to clockwise).

**arcTo(x1, y1, x2, y2, radius)**

Draws an arc with the given control points and radius, connected to the previous point by a straight line.


**quadraticCurveTo(cp1x, cp1y, x, y)**

Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.

**bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)**

Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).

**rect(x, y, width, height)**

Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.

![](https://mdn.mozillademos.org/files/245/Canvas_rect.png)

## Path2D objects

The Path2D() constructor returns a newly instantiated Path2D object, optionally with another path as an argument (creates a copy), or optionally with a string consisting of SVG path data.


Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

* fillStyle = color

Sets the style used when filling shapes.

* strokeStyle = color
Sets the style for shapes' outlines.

![color](https://mdn.mozillademos.org/files/5417/Canvas_fillstyle.png)


**globalAlpha = transparencyValue**

Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

The globalAlpha property can be useful if we want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors.

Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them.

There are several properties which allow us to style lines.

* lineWidth = value

Sets the width of lines drawn in the future.

* lineCap = type
Sets the appearance of the ends of lines.

* lineJoin = type
Sets the appearance of the "corners" where lines meet.

* miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

* getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.

* setLineDash(segments)
Sets the current line dash pattern.

* lineDashOffset = value
Specifies where to start a dash array on a line.

**createLinearGradient(x1, y1, x2, y2)**

Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).

**createRadialGradient(x1, y1, r1, x2, y2, r2)**

Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.

**createConicGradient(angle, x, y)**

Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

* createPattern(image, type)
Creates and returns a new canvas pattern object. image is a CanvasImageSource (that is, an HTMLImageElement, another canvas, a <*video>* element, or the like. type is a string indicating how to use the image.

The type specifies how to use the image in order to create the pattern, and must be one of the following string values:

* repeat
Tiles the image in both vertical and horizontal directions.
* repeat-x
Tiles the image horizontally but not vertically.
* repeat-y
Tiles the image vertically but not horizontally.
* no-repeat
Doesn't tile the image. It's used only once.

Using shadows involves just four properties:

* shadowOffsetX = float
Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

* shadowOffsetY = float
Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

* shadowBlur = float
Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.

* shadowColor = color
A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.


When using fill (or clip and isPointInPath) we can optionally provide a fill rule algorithm by which to determine if a point is inside or outside a path and thus if it gets filled or not. This is useful when a path intersects itself or is nested.

Two values are possible:

* "nonzero": The non-zero winding rule, which is the default rule.
* "evenodd": The even-odd winding rule.

Drawing text
The canvas rendering context provides two methods to render text:

* fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

* strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

* font = value

The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

* textAlign = value
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

* textBaseline = value
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

* direction = value
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

* measureText()
Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style.

![taex](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text/baselines.png)