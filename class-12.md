Apparently charts > tables for displaying data visually

Chart.js = a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.
  1. it’s simple to use and really very flexible. Plus, once you’ve mastered the basics here, you’ll discover that there are tons of options listed in the documentation.

The Canvas Element: has opening and closing tags and only has two attributes: width & height; these should be established inside the opening element tag, not in css and the format does not require px only something like width="200" height="200". Id and class attributes can also be put into the canvas element but are not necessary.
  1. The canvas element creates a fixed-size drawing surface that exposes one or more rendering contexts.
    1.a. The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The <canvas> element has a method called               getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered         by this tutorial, you specify "2d" to get a CanvasRenderingContext2D
  2. Fallback content: should the canvas not get rendered by the browser there should be some kind of fallback content between the opening and closing canvas tags.
  
You can also draw inside the canvas element, but you shouldn't because it seems like a lot more trouble than it's worth.
  1. You can also color and style these drawings in a vareity of ways, but again, there's gotta be easier ways of doing this.
  2. You can also 'draw text' and subsequently style said drawn text, but this doesn't seem any easier or prettier than simply adding text and styling it in CSS.
