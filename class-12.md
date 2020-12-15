## Drawing Paths:

A path is a list of points, connected by segments of lines that can be different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1. Create the path
1. Use drawing commands to draw into the path
1. Once the path has been created, you can stroke or fill the path to render it.

- beginPath()
Creates a new path. Once cread, future drawing commands are directed into the path and are used to build the path up.
- Path methods
Methods to set different paths for objects.
- closePath()
Adds a straight line to the path, going to the start of the currents sub-path.
- stroke()
Draws the shape by strokingit's outline.
- fill()
Draws a solid shape by filling the path's content area.

[Drawing Shapes with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

### Colors:

- fillStyle = color:
Sets the style used when filling shapes

- strokeStyle = color:
Sets the style for shapes' outlines.

Color is a string representing a CSS ``` <color>```, a gradient object, or a pattern object. By default the stroke and fill color are set to black.

[Applying Styles and Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

### Drawing Text:

- fillText(text, x, y, [, maxWidth]): Fills a given text at the given (x,y) position. Optionally with a maximum width to draw. 
- strokeText(text, x,y [, maxWidth]): Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

### Styling Text:

- font = value


The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

- textAlign = value

Text alignment setting. Possible values: start, end, left, right or center.  The default value is start.


- textBaseline = value

Baseline alignment setting. Possible values: top, haninging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.


- direction = value

Directionally. Possible values: ltr, rtl, inherit. The default value is inherit.



[Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)



[Basic Usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

[Chart.js docs](https://www.chartjs.org/docs/latest/)

[Chart.js API](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

[<----Back to Home](README.md)