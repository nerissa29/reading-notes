
## Reading Notes 12

### JavaScript Canvas

#### What does the canvas allow a developer to achieve?

The canvas element is an HTML5 feature that allows the user to draw 2D graphics through JavaScript. It has two attributes - (1) width, and (2) height, which can be access through the following[^1]:
  

```
<canvas width="500" height="300" id="canvas"></canvas>
```

Through DOM:

```
const canvas = document.querySelector('#canvas');
const width = canvas.width;// 500
const height = canvas.height;// 300
```

```
canvas.width = 600;
canvas.height = 400;
```

#### What is the importance of the closing canvas tag?

In between the opening and closing tags of canvas, lies the fallback content, which will be displayed in any case the browser does not support the canvas element[^1].


#### Explain what the getContext() method does.

The getContext() method is another feature of canvas element that returns "a render context object"[^1]. It takes the type of context as its one argument[^1]. 


### Chart.js Documentation

#### What is Chart.js and how it can be brought into your project?

It is a flexible tool used by the designers and developers for charting. It is used for "making HTML-based charts[^2]". Its built-in chart types are as follows[^2]:

- Scatter Plot
- Bar chart
- Line chart
- Bubble chart
- Donut Chart
- Pie chart
- Radar chart
- Area chart
- Mixed chart


#### List 3 different Chart types you can create using Chart.js.

As mentioned above, adapted from W3Schools page, below are the built-in chart types for chart.js[^2]:

- Scatter Plot
- Bar chart
- Line chart
- Bubble chart
- Donut Chart
- Pie chart
- Radar chart
- Area chart
- Mixed chart


### Easily Create Stunning Animated Charts with Chart.js

#### What are some advantages to displaying data via a chart over a table?
 One of the advantages the chart has is it conveys data quickly and are easier to use[^3]. It shows data in patterns, it can also show the relationships between different variables in graphs. Graphs or charts make it easier to read and remember than the statistics displayed in tables.

#### How could Chart.js aid your previously created applications visually?

It will make the data or the results easier to read in charts or graphs, rather than in lists. The differences and the relationships between the varaibles (voting count or views for example) can be spotted easily, compared to being written in unordered lists.


[^1]: [JavaScript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)
[^2]: [Chart.js](https://www.w3schools.com/js/js_graphics_chartjs.asp)
[^3]: [EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)







