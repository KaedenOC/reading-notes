# Problem Domain, Objects, and the DOM

[JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

## Object

A collection of related data and/or functionality. These usually consist of several variables and functions (which are called properties and methods when they are inside objects).

> Note: key/value pairs. Created with curly brackets. Creating an object often begins with defining and initializing a variable.

## Object Literal

List of value pairs inside curly brackets. The values can be properties and functions. It is common to create an object using an object literal when you want to transfer a series of structured, related data items in some manner.

## Objects Vs. Arrays

Objects map strings to values in the same way that arrays map numbers to values.
**Objects** are used to represent a "thing". person, a car, a building, a book, a character in a game etc. These are called properties that consist of a key and a value. **Arrays** we use when we want to create and store a list of multiple items in a single variable.

> Note: 

## Dot, and Bracket Notation

### Dot Notation

We access the object's properties and methods using dot notation. Object name must be entered first to access anything inside the object. Next you write a dot, then the item you want to access — this can be the name of a simple property, an item of an array property, or a call to one of the object's methods.

> Ex: person.age; person.bio();

### Bracket Notation

Provides an alternative way to access object properties. This looks very similar to how you access the items in an array, and it is basically the same thing — instead of using an index number to select an item, you are using the name associated with each member's value.

> Ex: person["age"]; person["name"]["first"];

## This

The "this" keyword refers to the current object the code is being written inside. When you only have to create one object literal, "this" isn't too useful. With more than one, "this" enables you to use the same method definition for every object you create.

> Ex: Questions 5. The term "this" is referring to the name value "spot", useful when creating more than one object from a single object definition.

## DOM

[Introduction To The DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

**Document Object Model** - Data representation of the objects that comprise the structure and content of a document on the web. Programming interface for web documents.

### DOM and JavaScript

The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, SVG documents, and their component parts. The DOM is not part of the JavaScript language, but is instead a Web API used to build websites.