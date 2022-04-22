---
layout: post
title:  "Blog 21 - jQuery"
date:   2022-4-21 5:15:29 -0700
categories: Tech
---
## jQuery: An Introduction 
The JavaScript library implemented for HTML DOM resource simplification is jQuery. This library makes features such as event handling, CSS animation, tree traversal and etc. easier for developers, and is an open-source software that is free. jQuery is used on about 73% of the "10 million most popular sites" according to W3Techs, and it has up to 4x more usage than any JavaScript library available. This is due to the simple syntax involved in jQuery which makes document navigation easy, along with providing capabilities for plug-ins on behalf of developers. Abstractions can be created through jQuery with the purpose of low-level interactions and animations which allow for widgets and advanced effects. This also leads to the creation of web pages and applications that are powerfully dynamic. To review more about jQuery in this blog, we will be touching upon its features, interface, and its pros and cons in implementation. 
<br/><br/>
<img src="https://miro.medium.com/max/1400/1*NeKYs9ypQ7jkalNxEX3t9Q.png" alt="MSC" width="300" height="150">
<br/>

## jQuery: Features
At its core level, jQuery is a library prepared for the manipulation of the Document Object Model (DOM). The tree-structure model of all web-page elements is referred to as the DOM, and jQuery enables simple syntax for manipulating elements within the DOM. An example of jQuery features include finding elements in the DOM with specific properties, such as all elements with the `h2` tag, or making a web page respond to a `keyboard click`. The main principles following jQuery's implementation reside in the separation of JavaScript and HTML, along with extensibility and elimination of cross-browser incompatibilities. The features listed below are just a glimpse of those offered by jQuery:
<br/><br/>
- `Ajax`: Ajax refers to the set of web-development techniques that are used on the client-side for web applications that are asynchronous. It is a programming concept that is a features available through jQuery. 
- `JSON parsing`: The open standard file format known as JSON can be parsed through a feature available in jQuery. This allows for the storing and transmitting of data objects that include arrays and attribute value pairs. 
- `Compatibility  Methods`: Compatibility methods are native in new browsers, but those that need fallbacks for safety can use methods such as `jQuery.each()` and `jQuery.inArray()`.
- `DOM manipulation`: As stated in the introduction, this feature is the most significant that jQuery has to offer, as it allows modification and manipulation of elements within the document object model. 

## jQuery: Interface
The jQuery Interface revolves around functions, which are split into jQuery object methods and static utility functions. These functions have their own style an can be accessed using the `jQuery` identifier. The jQuery Methods function is referred to as a `factory` as it allows the representation of one or multiple DOM nodes. The methods, also called commands, can be used to manipulate nodes in the DOM, and they are also chainable. Static utilities in the jQuery interface are utility functions and are accessed as static methods. An example would be `$.ajax()`, which calls a static method within the Ajax feature. 
<br/><br/>
There is a `no-conflict` mode in Jquery which can retrieve control of the `$`, which is an alias that refers to the jQuery identifier. This can be used in web page linking that needs the `$` symbol for identifiers. Using the no-conflict mode allows developers to use `jQuery` as a replacement for the alias without risking functionality within the webpage. As noted earlier, chaining is also part of the object methods interface feature as it enables the use of method chains. This allows developers to classify elements with attributes and retrieve specific values. 
<img src="https://www.tutorialspoint.com/jqueryui/images/jqueryui_category.jpg" alt="MSC" width="350" height="200">
<br/>

## Advantages and Disadvantages
The advantages of using jQuery start with its ease of use, as it is more easy to implement that standard javascript and other libraries within. Its large library size and strong opensource community are also very beneficial to new and current developers that employ jQuery. Ajax support is also a significant reason developers turn to Jquery as it enables a sleek interface to perform fast actions and not wait on the full page to reload before use. Great documentation is also available on jQuery as it is the most commonly used JavaScript library available. 
<br/><br/>
Some of the disadvantages associated with Jquery relate to limited functionality, as it is obviously not as versatile compared to the raw version of JavaScript. The javascript file being required is also a disadvantage in jQuery as it is necessary for the file to be present when running jQuery commands. Although the file size may be very tiny, (around 25-1000kb in size), it is still a file that has to be present on the client computer or web server.

### Learn More About jQuery
To learn more about jQuery visit their [website][web-io], to navigate blogs, plugins, browser support and etc. The jQuery [learning center][learn-io] includes an introduction as well as the most essential package introduction and tutorials to get started with jQuery. The jQuery [API][apidocuments-io] page also offers an interesting look into API Documentation including a set of definitions and protocols for building and integrating jQuery. 
<br/><br/>
Stay tuned for a new blog post next week!

[web-io]: https://jquery.com/
[apidocuments-io]: https://api.jquery.com/
[learn-io]: https://learn.jquery.com/
