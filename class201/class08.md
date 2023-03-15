# Layout With CSS

## Flexbox

[Learn-CSS Flexbox](https://web.dev/learn/css/flexbox/)

The **Flexible Box Layout Model** (flexbox) is a layout model designed for one-dimensional content. It excels at taking a bunch of items which have different sizes, and returning the best layout for those items.

Instead of setting rigid dimensions for the browser to follow, with flexbox, you can instead provide flexible boundaries to hint how the content could display.

### Features

- They can display as a row, or a column.
- They respect the writing mode of the document.
- They are single line by default, but can be asked to wrap onto multiple lines.
- Items in the layout can be visually reordered, away from their order in the DOM.
- Space can be distributed inside the items, so they become bigger and smaller according to the space available in their parent.
- Space can be distributed around the items and flex lines in a wrapped layout, using the Box Alignment properties.
- The items themselves can be aligned on the cross axis.


## Main Axis and Cross Axis

The **main axis** is the one set by your *flex-direction* property. If that is *row* your main axis is along the row, if it is *column* your main axis is along the column.

Flex items move as a group on the main axis. The cross axis runs in the other direction to the main axis.

The children of our flex container become flex items as soon as their parent gets display: flex, so these initial values mean that we start seeing some flexbox behavior.

## Accessibility

Any properties that reorder the visial display away from how things are ordered in the html document can negatively impact accessibility. The *row-reverse* and *column-reverse* values are examples.

[CSS Layout - Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

## Why Flexbox?

Floats and positioning can work but are limiting.

These exampls are considered difficult to achieve using floats and positioning.

- Vertically centering a block of content inside its parent.
- Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
- Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

I think Flexbox will be an important tool for many of my projects in the future. It seems incredibly useful for taking items of different sizes and returning the best layout for those items.