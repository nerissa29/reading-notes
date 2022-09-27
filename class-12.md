
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

[^1]: []()
