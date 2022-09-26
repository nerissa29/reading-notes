## Reading Notes 11

### Video and Audio Content

#### Explain how the ability to use video and audio on the web has evolved since the early 2000s.

The *video* element " embeds a media player which supports video playback into the document", an HTML Demo for *video* element is shoen below[^1]:

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

The *video* element works the same as the *img* element, a path to the media is included and placed inside the *src* attribute, other attributes like *width* and *height* can be specified as well.


The *audio* HTML element "is used to embed sound content in documents" and can have more than one audio sources as shown in the demo below[^2]: 

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

The *audi*, just like the *video* element, also works the same as the *img* element, where a media path is placed inside the *src* attribute, and can also specify whether we want the audio or  video to autoplay or loop.


[^1]: [Video: The Video Embed element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video)
[^2]: [Audio: : The Embed Audio element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio)
