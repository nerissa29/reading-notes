## Reading Notes 2

## Introduction to HTML

### Why is it important to use semantic elements in our HTML?

The *semantic HTML* provides the meaning of its elements to the developers and the browsers, allowing the browser know how to properly display it[^1]. Some of the semantic elements include:

```
<article>
<form>
<table>

```

The elements above describes its contents compared to *span* or *div*.

### How many levels of headings are there in HTML?

There are six headings level available in HTML:

```
<h1> A top-level heading </h1>
<h2> Second-level heading </h2>
<h3> Third..</h3>
<h4> Fourth..</h4>
<h5> Fifth..</h5>
<h6> The lowest-level heading </h6>

```

### What are some uses for the *sup* and *sub* elements?

The *sup* element "specifies inline text which is to be displayed as superscript for solely typographical reasons"[^2]. 

An example provided by MDN[^2]:

```
<p><var>a<sup>2</sup></var> + <var>b<sup>2</sup></var> = <var>c<sup>2</sup></var></p>


```
Results to: **a2 + b2 = c2**

The *sub* element "specifies inline text which should be displayed as subscript for solely typographical reasons"; an example is shown below[^3]:

```
molecule is
C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>, also known as "caffeine."</p>

```
Results to: **Almost every developer's favorite molecule is C8H10N4O2, also known as "caffeine."**


[^1]: [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
[^2]: [Sup: The Superscript Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sup)
[^3]: [Sub: : The Subscript Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sub)


