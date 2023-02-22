# Styling With CSS 🎨

## What Is CSS?

CSS allows you to create great-looking web pages. With CSS you can control how you want your HTML to be presented in the browser. you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

> CSS: Cascading Style Sheets. CSS is a language for specifying how documents are presented to users. It is a rule-based language.

## What Is The Purpose Of CSS?

CSS can be used for very basic document text styling. 

> Note: CSS can be used for changing the color, and size of headings and links. It can also be used for effects such as animation.

## CSS Selector

CSS selectors are the opening of the syntax. This selects the HTML element that we are going to style.

> EX: < h1> (no spaces)

## CSS Declaration

A set of curly brackets will hold one or more declarations in the form of **property** and **value** pairs.

> Ex: {color:red;} color is the property, and red is the value.

> CSS stylesheets will contain many rules, writtien one after another.

[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

## Three Ways To Insert CSS

There are three ways to insert CSS into your document.

* External CSS
* Internal CSS
* Inline CSS

## External CSS

You can change the look of an entire website by using one file.

> Note: Each HTML page must include a reference to the external style sheet file. The external .css file should not contain any HTML tags.

> Ex: (no spaces) < link rel="stylesheet" href="mystyle.css">

## Internal CSS

An internal style sheet may be used if one single HTML page has a unique style.

> Note: The internal style is defined inside the < style> (no spaces) element, inside the head section.

> Ex: (no spaces) < style>
body {
    background-color: red;
}

## Inline CSS

An inline style may be used to apply a unique style for a single element.

> Note: To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

> Ex: (no spaces) < h1 style="color:blue;>< /h1>

## Example CSS rule

> Ex: Make all paragraph elements text color red.
<br>p {color: red;
}