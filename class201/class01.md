# Developter Toolbelt

## How The Web Works

![clientserver](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works/simple-client-server.png)

*Clients* = users devices connected to the internet.<br>
*Servers* = computers that store webpages, sites, or apps.

> **Client** wants access to webpage<br>
> The webpage is then copied and downloaded from the **server** to be displayed to the user. 

- **Internet Connection** - Send and receive data on the web.
- **TCP/IP** - Stands for Transmission Control Protocol and Internet Protocol. These are communication protocols.
- **DNS** - Domain Name System. The browser looks at this to find a websites IP address. Find what server the website is from.

> Think of: Address Book.

- **HTTP** - HyperText Transfer Protocol. Application-layer protocol. Designed for communication between web browsers and servers.

## What Happens When We Type A Web Address Into The Browser?

1. Browser to DNS server to find the address.
2. **HTTP Request**. Which requests the server to send a copy of the website to the client. This is sent across users internet connection using TCP/IP.
3. If request is approved, the server sends the sites files to the browser in data packets.
4. Browser assembles the data packets and displays the web page.

### Parsing HTML, CSS, and JavaScript

The browser will parse the HTML first looking for any link elements containing CSS style sheets and/or JavaScript scripts.

> Note: The browser will send requests to the server regarding whether CSS and/or JavaScript is found.

Browser builds DOM tree, applies styles from CSSOM tree and executes the JavaScript.

## Images For Webpages

Find the image you would like for your webpage by using Googles search engine.

1. In order to avoid copyright violations, you can use things like Googles license filter to change the usage rights.

>Tools button --> Usage rights --> Creative Commons License.

2. You can save the image, and/or copy the images web address.

## Variables In JavaScript

Ways to declare a JavaScript variable:

- using **var**
- using **let**
- using **const**
- using nothing

What are Variables?

> Variables are containers for storing data (storing data values).

> Ex: x, y, and z, are variables, declared with the var keyword:<br>
var x = 5;
var y = 6;
var z = x + y;

We want to use Variables because they hold data values. These values can change meaning we can be dynamic.

**String** = sequence of text. Enclose in single or double quotes.

> Ex: let myName = 'kaeden'; or let myName = "kaeden";

**Number** = numbers dont have quotes.

> Ex: Numbers do not have quotes. let myAge = 25;

## Introduction To HTML

**Attributes** - Give more information about elements.

Attributes are followed by an equal sign.

Should also have an attribute value after the equal sign that is wrapped in double quotes.

> Ex: class=""

### Anatomy of an HTML Element

> opening tag, content, and closing tag

The *opening tag* is the name of the element, and is wrapped in brackets.

The *content* is everything inbetween the opening tag and closing tag.

The *closing tag* same as opening tag but includes a forward slash before the name of the element. This is where the element ends.

### Article Vs Section

**Article** - Used for wrapping similar content.

**Section** - Used more for grouping together a single part of a page.

### Elements That Are Typically Found In A Webpage

The elements that are commonly used in websites are:

> header, navigation bar, main content, sidebar, and footer.

## Metadata and SEO

Metadata is found in the head of the document which is not displayed in the web browser.

Metadata desriptions of content within the page can help with the pages SEO (Search Engine Optimization). These descriptions should include keywords from the web page.

> Ex: < meta charset="utf-8" /> found in the head element of the page.

## Designing A Website

When designing a website we want to think about:

- What we want plan to accomplish.
- our goals.
- what needs to be done, and in what order?

*Project Ideation*

> Note: It is considered good practice to draw out a Webframe once you have thought about what you want to accomplish with your website.

It is important to have a vision of what you want and how to get there.

WHAT DO YOU WANT TO ACCOMPLISH?

## Semantics

Semantics refers to the meaning of the code. The meaning or purpose of what things do.

An **h1** element, in most browsers, will be styled with a large font size to look like a heading.

**span**  can get styled to look like an h1 element but does not share the semantic value that h1 has.

It is important to use semantic tags in our HTML because:

- of important keywords for SEO.
- visually impaired can use screen readers to navigate the page.
- its easier to find meaningful blocks of code compared to looking through divs.
- of data population.
- of proper element/component naming.

## JavaScript

We use JavaScript to build complex ineteractive websites, browser games, and to connect servers to websites and web applications.

### How To Add JavaScript To The Page

In able to add JavaScript to the HTML, we can use inline JavaScript or External.

*Inline* - Like adding inline CSS but instead uses a **script** element.

*External* - Similar to adding external CSS. Create a new js file (script.js), and then place into the HTML head.

> Ex: < script src="script.js">< /script>