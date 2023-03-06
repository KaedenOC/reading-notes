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

>Ex: x, y, and z, are variables, declared with the var keyword:<br>
var x = 5;
var y = 6;
var z = x + y;

We want to use Variables because they hold data values. These values can change meaning we can be dynamic.

**String** = sequence of text. Enclose in single or double quotes. 

> Ex: let myName = 'kaeden'; or let myName = "kaeden";

**Number** = numbers dont have quotes.

> Ex: Numbers do not have quotes. let myAge = 25;

