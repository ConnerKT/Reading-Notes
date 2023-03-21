# Chart.js, Canvas

This topic is important to me because I want to discover more important ways to display data.

## References

<https://www.javascripttutorial.net/web-apis/javascript-canvas/>.
<http://www.chartjs.org/docs/>.
<https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/>.
<https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes>.
<https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors>.
<https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text>.

## JavaScript Canvas

The canvas element allows you to draw 2D graphics using JS.

It requires two attributes:width and height.

You can access it in DOM like so:

    const canvas = document.querySelector('#canvas');
    const width = canvas.width;// 500
    const height = canvas.height;// 300

The canvas tag uses the getContext() method that returns a render context obj.

The getContext() takes one argument which is the type of context. For example, you use the "2d" to get a 2D rendering context object, which is an instance of the CanvasRenderingContext2D interface.

This allows you to draw shapes, text, images ,and more.

    let canvas = document.querySelector('#canvas');
    let ctx = main.getContext('2d');

The fill and stroke properties of the 2d drawing context will determine the fill and stroke styles.

    (() => {
    const canvas = document.querySelector('#main');
    if (!canvas.getContext) {
        return;
    }

    // get the context
    let ctx = canvas.getContext('2d');

    // set fill and stroke styles
    ctx.fillStyle = '#F0DB4F';
    ctx.strokeStyle = 'red';

    // draw a rectangle with fill and stroke
    ctx.fillRect(50, 50, 150, 100);
    ctx.strokeRect(50, 50, 150, 100);

    })();

### JavaScript Canvas Questions

1. It allows a developer to draw 2d graphics onto a page.
2. It allows the fallback info to be contained in case a browser doesn't support canvas.
3. It allows us to return a rendered object.

## Chart.js Documentation

Chart.js is one of the most popular libraries.
It provides a set of frequently used chart types, plugins, and customization options.
It provides plugins to create annotations, zoom, or drag-and-drop functionalities to name a few things.
Canvas renders on the canvas tag, which allows it to be very performant.
Well suited for large datasets.

### Chart.js Documentation Questions

1. Its a popular JS library that allows you to create charts and helps it look nice. It can be brought in through the src tag.
2. Donut, Line, Bar.

## Easily Create Stunning Animated Charts with Chart.js

<https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/>.

In this link it describes the process of creating a chart.js chart, and its relatively easy. It isn't difficult to reproduce, and its easily designed with animations.

### Questions for Chart.js Animated

1. It can be more visually better, and it conveys data easier.
2. It can help present my data better visually without it being an hassle. And the data will be conveyed better with animations.

## Things I want to know more about

I want to know more about charting data.
I want to learn more about the animation aspect of chart.js.