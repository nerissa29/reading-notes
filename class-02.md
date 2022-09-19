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

The ***sup*** element "specifies inline text which is to be displayed as superscript for solely typographical reasons"[^2]. 

An example provided by MDN[^2]:

```
<p><var>a<sup>2</sup></var> + <var>b<sup>2</sup></var> = <var>c<sup>2</sup></var></p>


```

The *sup element* can also be used in ordinal numbers, such as 5th, 6th, 7th.


The ***sub*** element "specifies inline text which should be displayed as subscript for solely typographical reasons"; an example is shown below[^3]:

```
molecule is
C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>, also known as "caffeine."</p>

```

The *sub* element should only be used for typographical reasons and not for style. For styling purposes, CSS properties, such as *vertical-align* should be used.

Sub element can be used in footnote numbers, "marking up the subscript in mathematical variable numbers", or in specifying the number of atoms in chemical formulas[^3].


### When using the *abbr* element, what attribute must be added to provide the full expansion of the term?

The *abbr element* represents an acronym or abbreviation; when used, it is advisable to include the full text in plain text, along with the *abbr*, as shown in the image below[^4]:

<img width="373" alt="image" src="https://user-images.githubusercontent.com/113204667/191044915-57557f6a-9b3b-40ef-a2b0-f56cfc631b9d.png">
[HTML Demo](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/abbr)
doesn't exist.

The *title attribute* provides an expansion for the acronym or abbreviation, in any case, full expansion doesn’t exist.

## Learn CSS

### What are ways we can apply CSS to our HTML?

CSS can be applied through:
- External stylesheet
- Internal stylesheet
- Inline styles

The ***external Stylesheet*** is a separae file that has a .css extension, which contains the CSS styling. A singleCSS file - *external stylesheet*, can be link and used up to more than 1 web pages. To reference the this stylesheet, place the CSS file inside the *link* element as shown below[^5]:

```
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>

```

The ***internal stylesheet*** are written inside the HTML document. It is written an dplaced inside the *style element* which is found inside the HTML *head*[^5]:

```
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first CSS example</p>
  </body>
</html>

```

The *internal stylesheet* are less useful and can't be linked to more than one page. To use the same internal stylesheet on multiple pages, each page must have the same internal stylesheet written inside the *style element*.


The ***inline styles*** "are CSS declarations that affect a single HTML element, contained within a *style attribute*". It is considered the least efficient CSS implementation for maintenance; having the code and content separated from each other, makes it easier for the people who work on the website[^5].


An example adapted from MDN[^5]:

```
<!DOCTYPE html>
<html lang="en-GB">
  <head>
    <meta charset="utf-8" />
    <title>My CSS experiment</title>
  </head>
  <body>
    <h1 style="color: blue;background-color: yellow;border: 1px solid black;">
      Hello World!
    </h1>
    <p style="color:red;">This is my first CSS example</p>
  </body>
</html>

```

### Why should we avoid using inline styles?

According to MDN[^5]:
- it is less efficient when it comes to maintenance; it will be harder to read and understand if code and content are put together
- separating the web page content and its code makes it much easier for those who are working on the website
- Inline styles are prioritized first, before internal and external; a change in one style might end up needing multiple edits


### Review the block of code below and answer the following questions:

<img width="347" alt="image" src="https://user-images.githubusercontent.com/113204667/191053061-adac74b7-f006-476b-876e-0f63c86ce30d.png">
[Image from Read:Class 02](https://canvas.instructure.com/courses/5195147/discussion_topics/15584566)

### What is representing the selector?
- h2

### Which components are the CSS declarations?
- {
  }
  
### Which components are considered properties?
- color: ;
- padding: ;


## Learn JavaScript

### What data type is a sequence of text enclosed in single quote marks?
- String is a datatype wrapped around a single quote marks '' [^6]

### List 4 types of JavaScript operators
According to MDN[^6]:
- Addition (++)
- Subtraction, Multiplication, Division (-, *, /)
- Assignment operator (=)
- Strict equality (===)
- Not, Does-not-equal (!, !==)



[^1]: [Introduction to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)
[^2]: [Sup: The Superscript Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sup)
[^3]: [Sub: : The Subscript Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/sub)
[^4]: [Abbr: : The Abbreviation element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/abbr)
[^5]: [How CSS is structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)
[^6]: [JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)


