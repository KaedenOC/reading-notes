# Images, Color, Text, and More Work With Functions

Without a **src** attribute, an img element has no image to load.

the **alt** attribute is a textual description of the image. If the image cannot be seen/displayed or takes a long time to render, the text will show the user text.

Captions and alt text have distinct roles. Captions benefit even people who can see the image, whereas alt text provides the same functionality as an absent image.
> figcaption and alt

**figure** - could be several images, a code snippet, audio, video, equations, a table, or something else.

**SVG** - Ideal for user interface elements, icons, diagrams, etc., that must be drawn accurately at different sizes.

**GIF** - Simple images and animations.  GIF was one of the first two graphics formats supported by HTML

**Screenshots** - Should use a lossless format, PNG is best bet but WebP for better compression.

## More CSS

The **color** property defines the foreground color of an HTML element's content and the **background-color** property defines the element's background color. These can be used on just about any element.

- We can use CSS or JavaScript to change an elements color.

- **Color Palletes** - Useful tool to pick base color and other colors to accompany it.

### Font

**Web safe fonts** - are known to be available on nearly all instances of the most used operating systems. Good idea to use these.

**font-weight** - will set how bold the text will be.

**font-size** -  length and size of font. Try to avoid setting the font size of container elements because the font size of an element is inherited from that elements parent element.

> Types: px, em, rem

- **1em** - is = to the font size set on the parent element of the current element.

- **1rem** - is = to the size set on the root element of the doc not the parent.

**font-style** - used to turn italic text on or off.

> Types: normal, italic, oblique

### Spacing

**letter-spacing** and **word-spacing** allow you to set the spacing between letters and words in text.