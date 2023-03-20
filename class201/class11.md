# Audio and Video in HTML; Domain Modeling Revisited

## Video and audio on the Web

[Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

The first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. Both of these had security and accessibility issues, and are now obsolete.

**< video>** -  allows you to embed a video.

**src** - attribute contains a path to the video you want to embed

**controls** - Include the browser's own control interface, or build your interface using the appropriate JavaScript API. Start and stop the media and volume.

**fallback content** - paragraph inside the video tag. will be displayed if the browser accessing the page doesn't support the video element, allowing us to provide a fallback for older browsers.

## CSS Grid

[A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

**CSS Grid** - two-dimensional grid-based layout system.  Completely changes the way we design user interfaces. Different from FlexBox because flex has a one-directional flow and has different use cases. Grid and Flex work together well.

1. Define a container element as a grid **display: grid**.
2. Set the column and row sizes.
**grid-template-columns** and **grid-template-rows**.
3. Place its child elements into the grid with **grid-column** and **grid-row**.

## Responsive Images

[Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

Images that work well on devices with widely differing screen sizes, resolutions, and other such features.

There is no need to embed such large images on the page if it is being viewed on a mobile screen. Doing so can waste bandwidth. We want to display identical image content, just larger or smaller depending on the device.

### srcset and sizes

**srcset** defines the set of images we will allow the browser to choose between, and what size each image is.

**sizes** defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true.

> Ex: < img
  srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
  sizes="(max-width: 600px) 480px,
         800px"
  src="elva-fairy-800w.jpg"
  alt="Elva dressed as a fairy" />

## Why Not CSS or JS?

In order to reduce the page load times, the browser loads the images before the main parser has started to load and interpret the page's CSS and JavaScript. You couldn't load the < img> element, then detect the viewport width with JavaScript, and then dynamically change the source image to a smaller one if desired.