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


## What is the Difference between the <article></article> and <section></setion> element tags?

The ***section tag***  allows user to create a section in the HTML document, while the ***article tag*** allows the user to create self-contained content. The ***section tag*** can divide or split the HTML page into sections. The ***article tag*** can be placed inside the ‘’’<main></main>’’’ or ‘’’<section></section>’’’; it works independently and does not require another context[^3].


## What Elements does a “typical” website include?
The HTML provides tags one can use to denote a section. Examples would be:
-	header - headear tag
-	Navigation bar - nav tag
-	Main content - main tag, which may also include subsections such as: (1) article tag, (2) section tag, (3) div tag
- sidebar - aside tag, which is also placed mostly inside the <main></main>
- footer - footer tag


## References:
[^1]: [How CSS works] (https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_works)
[^2]: [HTML Images] (https://www.w3schools.com/html/html_images.asp)
[^3]: [Difference between <article> tag and <section> tag] (https://www.geeksforgeeks.org/difference-between-article-tag-and-section-tag/#:~:text=The%20tag%20defines%20a,independent%2C%20self%2Dcontained%20content.)
- 
- 





  
