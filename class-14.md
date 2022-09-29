## Reading Notes 14

### CSS Transforms

#### What does a CSS transform allow the developer to do to an element?
 The CSS *transform property* has two settings: (1) two-dimensional, and (3) three-dimensional; the syntax is as follows[^1]:
 
 ```
 div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
 ```
 The specific amount is wrapped inside the parenthesis, and the value specifies its transform type; the two-dimensional transforms work on both the horizontal and vertical axes (x and y), while the three-dimensional transform works on both x, y, and z axes[^1].
 
 
 #### Provide an example of a transform and how you could see that being used on a website.
 
 One interesting sample provided on the website/article titled *Transforms* are as follows:
 
 ```
 HTML:
 
 <div class="cube">
  <figure class="side top">1</figure>
  <figure class="side left">2</figure>
  <figure class="side right">3</figure>
</div>
 
 ```
 ```
 CSS:
 
 .cube {
  position: relative;
}
.side {
  height: 95px;
  position: absolute;
  width: 95px;
}
.top {
  background: #9acc53;
  transform: rotate(-45deg) skew(15deg, 15deg);
}
.left {
  background: #8ec63f;
  transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
}
.right {
  background: #80b239;
  transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
}
 
 ```
 <img width="451" alt="image" src="https://user-images.githubusercontent.com/113204667/193062297-51ed37d8-d956-4daa-b83c-48bfc046cef8.png">
 
 
 
 [^1]: [Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)


