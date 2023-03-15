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

