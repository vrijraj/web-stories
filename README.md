# AMP Story
[AMP story](https://amp.dev/about/stories) is a full-screen visual storytelling experience that conveys information with images, videos, graphics, audio, and more. 

Check out the [Gradus Codelab](https://gradus.vrijraj.xyz/amp-web-stories?page=0)

## amp-story web component

<img src='https://amp.dev/static/img/docs/tutorials/amp_story/story_parts.png' width="100%">

<img src="https://amp.dev/static/img/docs/amp-story-tag-hierarchy.png" width="100%">

## Getting Started
1. Add `amp` js library in your web page
    ``` js
    <script async src="https://cdn.ampproject.org/v0.js"></script>
    ```
1. Import `amp-story` library in your web page
    ``` js
    <script async custom-element="amp-story"
        src="https://cdn.ampproject.org/v0/amp-story-1.0.js"></script>
    ```
1. So your web page look like
    ``` html
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Document</title>
            <script async src="https://cdn.ampproject.org/v0.js"></script>
            <script async custom-element="amp-story"
            src="https://cdn.ampproject.org/v0/amp-story-1.0.js"></script>
        </head>
        <body>
            <p>AMP Story</p>
        </body>
    </html>
    ```
1. `<amp-story>`, `<amp-story-page>`, `<amp-story-grid-layer>` in your story
    ```html
    <amp-story standalone >
        <amp-story-page id="cover">
            <amp-story-grid-layer template="fill">
                <amp-img src="/assets/a.jpg"
                    width="720" height="1280"
                    layout="responsive">
                </amp-img>
            </amp-story-grid-layer>
            <amp-story-grid-layer template="vertical" style="color:white">
                <h1 animate-in="fly-in-right">Google Developers Group</h1>
                <p animate-in="fade-in">Google Developer Groups (GDGs) are for developers who are interested in Google's developer technology.</p>
            </amp-story-grid-layer>
        </amp-story-page>
    </amp-story>
    ```


## Resources
1. [Gradus Codelab](https://gradus.vrijraj.xyz/amp-web-stories?page=0)
1. [AMP Story Docs](https://amp.dev/documentation/guides-and-tutorials)
