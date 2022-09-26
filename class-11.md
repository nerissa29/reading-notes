## Reading Notes 11

### Video and Audio Content

#### Explain how the ability to use video and audio on the web has evolved since the early 2000s.

The *video* element " embeds a media player which supports video playback into the document", an HTML Demo for *video* element is shown below[^1]:

```
<video controls width="250">

    <source src="/media/cc0-videos/flower.webm"
            type="video/webm">

    <source src="/media/cc0-videos/flower.mp4"
            type="video/mp4">

    Download the
    <a href="/media/cc0-videos/flower.webm">WEBM</a>
    or
    <a href="/media/cc0-videos/flower.mp4">MP4</a>
    video.
</video>

```

The *video* element works the same as the *img* element, a path to the media is included and placed inside the *src* attribute, and other attributes like *width* and *height* can be specified as well.


The *audio* HTML element "is used to embed sound content in documents" and can have more than one audio source as shown in the demo below[^2]: 

```
<figure>
    <figcaption>Listen to the T-Rex:</figcaption>
    <audio
        controls
        src="/media/cc0-audio/t-rex-roar.mp3">
            <a href="/media/cc0-audio/t-rex-roar.mp3">
                Download audio
            </a>
    </audio>
</figure>

```

The *audio*, just like the *video* element, also works the same as the *img* element, where a media path is placed inside the *src* attribute and can also specify whether we want the audio or video to autoplay or loop. Online videos and audios are first made possible by "plugin-based technologies like Flash and Silverlight"[^3], which has accessibility and security issues "and are now obsolete, in favor of native HTML solutions *video and audio* elements and the availability of JavaScript APIs for controlling them"[^3].
    
#### Describe the use of the src and controls attributes in the video element.

The *src* attribute embeds the video path; it works the same way as the *img* element[^3]. The *controls* is a way for a user to be able to control the video. The *control* attribute uses the "browser's own control interface", or one can build an interface " using the appropriate JavaScript API"[^3].


#### Why is it important to have fallback content inside the video element?

The fallback content is the paragraph shown below[^3]:

```
<video src="rabbit320.webm" controls>
  <p>
    Your browser doesn't support HTML video. Here is a
    <a href="rabbit320.webm">link to the video</a> instead.
  </p>
</video>

```

In any case the browser doesn't support the *video* element, the *fallback content* will display the message; it allows "to provide a fallback for older browsers"[^3]. A direct link can be provided so that the user can still have a way to access the video.


### A Complete Guide To Grid

#### How does Grid layout differ from Flex?

The Flexbox is a one-dimensional layout; it's layout is designed to be one-dimension, it could be a row or a column. Grid, on the othe other hand, is designed to be a two-dimensional layout, it can be both rows and columns at the same time[^4].


#### Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

The *display: grid | inline-grid;* property defines the element as a "grid container and establishes a new grid formatting context for its contents"[^5]. The *grid* "generates a block-level* grid, and the *inline-gris* "generates an inline-level grid"[^5]. A grid container can contain *grid items* which can be styled. The *grid line* are lines - (a) vertical or "column gridlines", (b) horizontal or "row grid lines", that make up the grid stucture[^5].




[^1]: [Video: The Video Embed element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)
[^2]: [Audio: The Embed Audio element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio)
[^3]: [Video and Audio content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)
[^4]: [Relationship of Grid Layout to Other Layout Methods](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout/Relationship_of_Grid_Layout#:~:text=already%20be%20using.-,Grid%20and%20flexbox,columns%20at%20the%20same%20time.)
[^5]: [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

