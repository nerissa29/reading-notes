## Reading Notes 5

###### Readings: Images, Color, Text

###### HTML Media

###### What is a real world use case for the alt attribute being used in a website?

The *alt attribute* is use to describe the image, in any case the image won't load, *alt* will give the reader a descriptiont of what the image is about. It is placed inside the *img tag*:

An example from MDN web docs[^1]:

```
<img scrc="images/dinosaur.jpg" alt="The head and torso of a dinosaur skeleton" />
      
```
Importance of ***Alt attribute***:
- with text description, it helps visually impaired user using a "screen reader to read the web out to them[^1]"
- when image is not supported by the browser or when path is wrong, the text description will let the user know about the image
- with search queries, the search engines can look into the alt text 
- useful when user has the images turned off 

###### How can you improve accessibility of images in an HTML document?


[^1]: [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
