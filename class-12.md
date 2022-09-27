
## Reading Notes 12

### JavaScript Canvas

#### What does the canvas allow a developer to acheive?

The canvas element is an HTML5 feature that allows the user to dra 2D graphics through JavaScript. It has two attributes - (1) width, and (2) height, which can be access through the following[^1]:
  

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


[^1]: [JavaScript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)
