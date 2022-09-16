## Reading Notes 5

#### Readings: Images, Color, Text

##### HTML Media

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

Aside from adding *alt attribute* that helps the search engines identifiy if the image matches the queries, ensuring images has it's correct path is important as well. These two increases the accessibility of the images to the users. In describing decorative images, use the empty alt tag instead (alt=''); also, adding desc[^2].

When adding captions, for easy reading, it s best to enclose the image to *figure* element instead of *div*[^1]:

```
<figure>
  <img
    src="images/dinosaur.jpg"
    alt="The head and torso of a dinosaur skeleton;
            it has a large head with long sharp teeth"
    width="400"
    height="341" />

  <figcaption>
    A T-Rex on display in the Manchester University Museum.
  </figcaption>
</figure>
```

###### Provide an example of when the figure element would be useful in an HTML document.

The *img* element can be enclosed inside the *div* element. However, if caption is needed, caption won't be semantically link to the image, due to *div* doesn't have a *figcaption* elements. A *p tag* can be used to wrap the text an serves as a caption, but it will not be semantically link to the image. On the other hand, using the *figure* element and *figcaption* element solves the issue. These two together are created to provide the caption semantically link to the image, see the difference below, adapted from MDN wed docs[^1]:

***div element***
```
<div class="figure">
  <img
    src="images/dinosaur.jpg"
    alt="The head and torso of a dinosaur skeleton;
            it has a large head with long sharp teeth"
    width="400"
    height="341" />

  <p>A T-Rex on display in the Manchester University Museum.</p>
</div>
```

***figure and figcaption element***
```
<figure>
  <img
    src="images/dinosaur.jpg"
    alt="The head and torso of a dinosaur skeleton;
            it has a large head with long sharp teeth"
    width="400"
    height="341" />

  <figcaption>
    A T-Rex on display in the Manchester University Museum.
  </figcaption>
</figure>
```



[^1]: [Images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
[^2]: [Make your Images Accessible](https://itaccessibility.arizona.edu/content/images)

