# Chart.js, Canvas

### Chart.js API
https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/

### Getting Chart.js documents.

https://www.chartjs.org/docs/latest/

### Basic use of canvas
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage

Canvas element - Use this element to provide a place from your js to apply your chart. This element has a width and height att. and you will want to supply this element with an id to access through js. You will need a closing tag as well.

Read article above for fallback content.

You canvas is blank, use code below. You need to use the getContext(). This will take only one parameter, the context type. In this case, '2d'.

        let canvas = document.getElementById('id of canvas element');
        let con = canvas.getContext('2d);

### Drawing shapes with canvas

https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes

canvas only supports two shapes, rectangles and paths. Paths are points connected by a line. Other shapes are must be made by combing two paths.

**Three functions that draw rectangles on canvas: see article**

### Draw Rectangles
The parameters of the fillRect(), strokeRect(), and clearRect are x,y,width,height. the x and y specify position within the canvas element and then specify the width and height of the rectangle.

### Draw paths

Create your path, use your draw commands to draw your path, the stroke or fill path to render.

Function to start: beginPath();

Then use path methods.

closePath() to 

stroke() draws shape by stroking outline

fill() solid shape drawn, fills path's content

You can draw arc, lines, triangles, rectangles, etc.

### Applying styles and colors 
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors

### Drawing Text
https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text

[code201Table](./201/code201Table.md)

[Back to Homepage](README.md)