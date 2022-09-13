# Reading Notes 1

## Describe how HTML, CSS, and JS files are “parsed” in the browser.

The browser loads the HTML and converts it into a Document Object Model or DOM[^1]. 
The browser will then fetch the resources linked to the HTML document; this could be embedded videos, images, or CSS. 
The browser parses and sorts the fetched CSS into different rules by their selector types, such as element, ID, class, and many more. 
It finds and works out the rules that need to be applied on nodes, .attaching the style to them


## How can you find images to add to a Website?

The img tag is used to embed an image into the web page; it links the images to the web page. The img tag creates as a placeholder for the referenced image. Two required attributes include[^2]:
-	Src – specifies the image’s path
-	Alt – an alternate text for the image


## How do you create a String vs a Number in JavaScript?

Strings in JavaScript can be written inside either the (1) single quotes(‘’), the (2) double quotes (“”), or the (3) backticks (``). The quotes style used must be the same on both sides. However, these three styles can be used throughout the HTML document as long as the beginning and ending of the style used are matching.

Strings can also be declared by using ***let***, which allows to declare variables, such as:
  let str = 'name'
  
Numbers can also be assigned to a variable, only this time, it's not enclosed in quotes.
  let num = 3
  
  
  
## What is a Variable and why are they important in JavaScript?

***Variables*** act like placeholders used to store values. Below is an example of declaring a variable:
```
let name = “Issa”;    
let str;   
```

The 1st example declares variable ***name*** and assigns it the String value ***Issa***. 
The 2nd example declares a variable ***str*** with a value ***undefined***, which can later have values. 
In addition, variables can hold values ‘that have different data types, such as[^4]:
- String
- Number
- Boolean
- Object
- Array



# Introduction to HTML

## What is an HTML attribute?

The 'HTML (HyperText MarkUp Language) is a markup language that tells web browsers how to structure the web pages you visit'[^5]. It consists of elements used to wrap or enclosed 'different parts of content to make it appear or act in a certain way'[^5]. 

On the other hand, the attributes hold additional pieces of information placed inside the opening tag. In the example below:

``` 

<img src = "flower.jpg" alt = "A State Flower."> 

```

The ***src*** and the ***alt*** serves as the <img> tag's attributes. It provides more details regarding the HTML element <img>.


## Describe the Anatomy of an HTMl element.

``` 

<h1> Code 201 </h1>

The opening tag <h1> and the closing tag </h1> is considered an element, while the text 'Code 201' is considered the content

```
- ***opening tag*** - is the name of the element, 'p for paragraph'[^5].
- ***content*** - is the element's content[^5].
- ***closing tag*** - it marks the ending, it is important to include closing tags to prevent error[^5]


        
## What is the Difference between the article and section element tags?

The ***section tag***  allows user to create a section in the HTML document, while the ***article tag*** allows the user to create self-contained content. The ***section tag*** can divide or split the HTML page into sections. The ***article tag*** can be placed inside the ***main or section tag***; it works independently and does not require another context[^3].


## What Elements does a “typical” website include?
The HTML provides tags one can use to denote a section. Examples would be:
-	```<header></header>```
-	```<nav></tag>```
-	```<main></main>```, which may also include subsections such as: (1) ```<article></article>```, (2) ```<section></section>```, (3) ```<div></div>```
- ```<aside></aside>``` - sidebar, which is also placed mostly inside the <main></main>
- ```<footer></footer>```


## How does metadata influence Search Engine Optimization?

'Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document’ — the ***meta*** element [^6]. Since metadata is written in a language that search engines understand, it, therefore, helps the search engines understand the content of the webpage.

```
<meta charset = "utf-8">

```
The ***utf-8*** is a universal character set that allows the web page to be able to handle any language displayed[^6]. It has a great impact on the search engines and SEO as it tells the page's title to the search engine 


## How is the meta HTML tag used when specifying metadata?

The ***meta tag*** defines the metadata - 'data that describes data' about the HTML document. It represents metadata that cannot be represented by either ***base, script, style, and many more***[^6]


'The type of metadata provided by the <meta> element can be one of the following[^7]:

- ***name*** attribute - provides the type of data applied to the web page. The *name* and it's *content* are used together for easy and right searches. The *name* attribute gives metadata a name, while the *content* attribute holds the value.

- ***http-equiv*** attribute -once set, provides HTML header for the *content* attribute's value

- ***charset*** attribute - encodes the character; UTF-8 is advised as it covers most characters and symbols.

- ***itemprop*** attribute - it provides user-defined metadata and must not be set with the same *meta* where *name, http-equiv, or charset* exists.



# Miscellaneous

## What is the first step to designing a Website?

Aside from the need-to-know how to build a website, having a goal is important, and also is the very first step. Once a goal is established, the next step will be defining the scope of the project, as well as designing the web page. Creating its content is the next development; the final step will be launching the website.
       

## What is the most important question to answer when designing a Website?

These three questions are important in designing a website:
- 'What exactly do I want to accomplish[^8]?'
- 'How will a website help me reach my goals[^8]?'
- 'What needs to be done, and in what order, to reach my goals?[^8]'




[^1]: How CSS works [Click here](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_works)
[^2]: HTML Images [Click here](https://www.w3schools.com/html/html_images.asp)
[^3]: Difference between article tag and section tag [Click here](https://www.geeksforgeeks.org/difference-between-article-tag-and-section-tag/#:~:text=The%20tag%20defines%20a,independent%2C%20self%2Dcontained%20content.)
[^4]: JavaScript Basics [Click here](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)
[^5]: Getting Started with HTML [Click here](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
[^6]: What's in the head? Metadata in HTML [Click here](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)
[^7]: The metadata element [Click here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta)
[^8]: [How do I start to design my website?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)





  
